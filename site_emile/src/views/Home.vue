<template>
  <div class="main">
    <div class="header">
      <h1 class="header-title">Créations sur bois</h1>
      <h2 class="header-subtitle">Fait main, sur-mesure pour particuliers</h2>
    </div>
    <h2 class="card-title">Mes Créations :</h2>
    <div class="card-container">
      <div class="product-card">
        <ProductCard
          v-for="product in products"
          :key="product.id"
          :products="product.name"
        />
      </div>
    </div>
  </div>
</template>

<script>
import ProductCard from "../components/ProductCard.vue";
export default {
  components: { ProductCard },
  data() {
    return {
      products: [
        {
          id: 1,
          name: "Décapsuleur Bois",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
        },
        {
          id: 2,
          name: `Enseigne "WALK"`,
          description: "Lorem ipsum dolor sit amet, consectetur",
        },
      ],
    };
  },
};
</script>

<style scoped>
.main {
  background-color: #272f5c;
  min-height: 100vh;
  color: #d96d0f;
}
</style>
