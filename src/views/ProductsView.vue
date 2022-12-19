<template>
  <h1>Products</h1>
  <hr>
  <Products/>
</template>

<script>

import Products from '../components/Products.vue'
export default {
  components: {
    Products
  }
}
</script>

<style scoped>
  hr {
    height: 30px;
    border-top: 2px solid black;
    width: 85%;
    margin: 25px auto;
  }
</style>