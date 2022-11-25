<script setup>
defineProps({
  ordered: {
    type: Boolean,
    default: false,
  },
  bullets: {
    type: Boolean,
    default: false,
  }
})
</script>

<template>
  <div class="container my-4 mx-4 max-w-lg md:mx-12">
    <ol v-if="ordered" class="list-decimal">
      <slot></slot>
    </ol>
    <ul v-else :class="bullets ? 'list-disc' : 'list-none'">
      <slot></slot>
    </ul>
  </div>
</template>