<template>
    <div class="text-component">
      <p>{{ text }}</p>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      text: {
        type: String,
        required: true
      }
    }
  };
  </script>
  
  <style scoped>
  .text-component {
    font-size: 16px;
  }
  </style>
  