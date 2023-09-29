<template>
    <div class="image-component">
      <img :src="imageUrl" alt="Image" />
    </div>
  </template>
  
  <script>
  export default {
    props: {
      imageUrl: {
        type: String,
        required: true
      }
    }
  };
  </script>
  
  <style scoped>
  image-component img {
  max-width: 10%; 
  height: auto;
}
  </style>
  