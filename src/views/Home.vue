<template>
  <h1>Home</h1>
  <div class="splash-container">
    <div class="splash">
      <h1>Splendid Food</h1>
    </div>
  </div>

  <main class="wrapper">

    <h2>Recommended</h2>

    <div class="recommended">

        <ProductCard
          v-for="(product, index) in inventory.slice(0,3)" 
          :key="product.id"
          class="card"
          :index="index"
          :product="product"
          :addToCart="addToCart"
        />

    </div>


  </main>
</template>

<script>
import ProductCard from '@/components/ProductCard';

export default {
  name: "Home-page",
  props: ['inventory', 'addToCart'],
  components: {
    ProductCard
  },
};
</script>
