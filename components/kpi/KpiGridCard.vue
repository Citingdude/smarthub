<script setup lang="ts">
const props = defineProps<{
  subtitle: string
  title: string
  description: string
}>()
</script>

<template>
  <div class="flex flex-col justify-center items-center p-16 gap-4 bg-light aspect-square">
    <p class="text-tertiary text-[20px] leading-[26px] font-light text-center">
      {{ props.subtitle }}
    </p>

    <p class="text-center text-primary font-bold font-display text-[45px] leading-[55px]">
      {{ props.title }}
    </p>

    <p class="text-tertiary text-[20px] leading-[26px] font-light text-center">
      {{ props.description }}
    </p>
  </div>
</template>
