<template>
  <header class="bg-white shadow-sm">
    <nav class="container flex justify-between p-4 mx-auto">
      <ul class="flex gap-4">
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/products" class="btn">Products</NuxtLink></li>
      </ul>
    </nav>
  </header>

  <div class="container p-4 mx-auto">
    <slot />
  </div>
</template>

<style scoped>
.router-link-exact-active {
  color: red;
}
</style>
