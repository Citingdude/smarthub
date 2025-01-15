<script setup lang="ts">
const props = defineProps<{
  to: string
  label: string
}>()
</script>

<template>
  <NuxtLink class="flex w-fit gap-2 items-center group" :to="props.to">
    <span class="text-lg font-display group-hover:text-secondary group-hover:underline transition">
      {{ label }}
    </span>

    <IconArrowRight class="fill-primary" />
  </NuxtLink>
</template>
