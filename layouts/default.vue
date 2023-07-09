<template>
  <div>
    <header>
      <nav>
        <div>Nuxt Link</div>
        <ul>
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
          <li><NuxtLink to="/products/123">Products 123</NuxtLink></li>
          <li><NuxtLink to="/products/456">Products 456</NuxtLink></li>
        </ul>
      </nav>
      <nav>
        <div>Normal Link</div>
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/about">About</a></li>
        </ul>
      </nav>
    </header>
    <div>
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