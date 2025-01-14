<script setup lang="ts">
import { tv } from 'tailwind-variants'

const props = defineProps<{
  label: string
  to: string
  color: 'primary' | 'white'
}>()

const button = tv({
  base: 'py-[14px] px-5 font-bold font-display text-lg rounded-full transition flex items-center gap-[10px] w-full sm:w-fit',
  variants: {
    color: {
      white: 'bg-white hover:bg-gradient-to-r hover:from-gradient-from hover:to-gradient-to text-dark fill-primary hover:fill-white hover:text-white',
      primary: 'bg-gradient-to-r from-gradient-from to-gradient-to text-white',
    },
  },
})
</script>

<template>
  <NuxtLink
    :to="props.to"
    :class="button({ color: props.color })"
  >
    <span>
      {{ props.label }}
    </span>

    <IconArrowRight />
  </NuxtLink>
</template>
