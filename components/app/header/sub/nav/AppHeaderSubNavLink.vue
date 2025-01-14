<script setup lang="ts">
const props = defineProps<{
  to: string
  label: string
}>()
</script>

<template>
  <li>
    <NuxtLink class="text-base hover:text-primary transition underline font-display" :to="props.to">
      {{ props.label }}
    </NuxtLink>
  </li>
</template>
