<template>
  <header class="shadow-sm">
    <nav class="container p-4">
      <NuxtLink class="font-bold" to="/products">Nuxt Dojo Merch</NuxtLink>
    </nav>
  </header>
  <!-- output the page content-->
  <div class="container mx-auto p-4">
    <slot />
  </div>
  <footer class="container mx-auto p-4 border-t-2">
    <ul class="flex gap-4">
      <li>
        <NuxtLink to="/">Home</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/about">About</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/products">Products</NuxtLink>
      </li>
    </ul>
  </footer>
</template>
<style scoped>
.router-link-active {
  color: green;
}
</style>
