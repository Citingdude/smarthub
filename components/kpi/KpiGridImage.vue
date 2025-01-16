<script setup lang="ts">
const props = defineProps<{
  src: string
  alt: string
}>()
</script>

<template>
  <div class="flex">
    <img
      class="aspect-square object-cover w-full h-auto"
      :src="props.src"
      :alt="props.alt"
    >
  </div>
</template>
