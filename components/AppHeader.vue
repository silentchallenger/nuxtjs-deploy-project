<script setup>
defineProps({
  pageTitle: {
    type: String,
    default: "Default Page Title",
  }
})
</script>
<template>
  <header class="container flex justify-center text-5xl font-bold p-4">
    <h1>{{ pageTitle }}</h1>
  </header>
</template>