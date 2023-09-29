<template>
    <div class="link-component">
      <a :href="url" target="_blank">{{ label }}</a>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      url: {
        type: String,
        required: true
      },
      label: {
        type: String,
        required: true
      }
    }
  };
  </script>
  
  <style scoped>
  .link-component a {
    color: blue;
    text-decoration: underline;
  }
  </style>
  