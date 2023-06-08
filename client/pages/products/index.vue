<template>
  <div>
    <div class="grid grid-cols-3 gap-5">
      <div v-for="p in products">
        <ProductCard :product="p" />
      </div>
    </div>
  </div>
</template>
<script setup>
definePageMeta({
  layout: "default",
});

const { data: products } = await useFetch("https://fakestoreapi.com/products");
</script>
