<template>
  <div class="mt-7 max-w-sm mx-auto card text-center">
    <p class="mt-7 text-7xl font-bold">{{ error.statusCode }}</p>
    <p class="mt-7 text-6xl">Ooops.</p>
    <p class="mt-7">{{ error.message }}</p>
    <button class="my-7 btn" @click="handleClearError">Go home...</button>
  </div>
</template>

<script setup>
defineProps(['error']);

const handleClearError = () => clearError({ redirect: '/' });
</script>

<style lang="scss" scoped></style>
