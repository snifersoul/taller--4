<template>
  <div class="info-component">
    <h2>{{ title }}</h2>
    <p>{{ description }}</p>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
.info-component {
  background-color: #f0f0f0;
  padding: 20px;
  border-radius: 10px;
}
</style>
