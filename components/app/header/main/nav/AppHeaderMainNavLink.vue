<script setup lang="ts">
const props = defineProps<{
  label: string
  to: string
}>()
</script>

<template>
  <li>
    <NuxtLink
      class="font-display text-[26px] font-bold text-right text-white hover:text-secondary transition" :to="props.to"
    >
      {{ props.label }}
    </NuxtLink>
  </li>
</template>
