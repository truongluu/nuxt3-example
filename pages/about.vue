<template>
  <h1>About</h1>
  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim laborum error
    cupiditate excepturi impedit veritatis magni debitis incidunt eius fugiat.
  </p>
  <p>{{ data }}</p>
</template>

<script setup>
const { data } = await useFetch('/api/ninja?name=ninja1', {
  method: 'post',
  body: { age: 15 },
});
</script>

<style scoped></style>
