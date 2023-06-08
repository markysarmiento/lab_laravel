<template>
  <div class="h-full p-3 text-center bg-white rounded-md shadow-md">
    <img :src="product.image" alt="product_thumb" class="thumb" />
    <p class="m-4 font-bold text-gray-500 truncate">Title: {{ product.title }}</p>
    <p class="m-4 font-bold text-gray-500 truncate">Price: ${{ product.price }}</p>
    <p class="m-4 font-bold text-gray-500 truncate">Category: {{ product.category }}</p>
    <NuxtLink :to="`/products/${product.id}`">
      <p class="my-4 btn">View Details</p>
    </NuxtLink>
  </div>
</template>

<script setup>
const { product } = defineProps(["product"]);
</script>

<style scoped>
  .thumb {
    max-height: 120px;
    max-width: 70%;
    margin: 0 auto;
  }
</style>
