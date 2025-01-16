<script setup lang="ts">
const props = defineProps<{
  label: string
  to: string
}>()
</script>

<template>
  <li>
    <NuxtLink class="font-display underline hover:text-secondary" :to="props.to">
      {{ props.label }}
    </NuxtLink>
  </li>
</template>
