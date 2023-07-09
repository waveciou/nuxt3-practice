<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4 flex justify-between">
        <div>Nuxt 3</div>
        <ul class="flex gap-4">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
          <li><a href="/">Normal - Home</a></li>
          <li><a href="/about">Normal - About</a></li>
        </ul>
      </nav>
    </header>
    <div class="container mx-auto p-4">
      <slot />
    </div>
  </div>
</template>

<script setup>
  // Use <slot> for the output of layout.
</script>

<style lang="scss" scoped>
  .router-link-exact-active {
    color: #12b488;
  }
</style>