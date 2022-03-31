<template>
  <div class="product-card">
    <h1 class="product-name">{{ name }}</h1>
    <p class="product-description">
      {{ description }}
    </p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      props: ["name", "description"],
    };
  },
};
</script>

<style scoped>
h1 {
  color: #d96d0f;
}
</style>
