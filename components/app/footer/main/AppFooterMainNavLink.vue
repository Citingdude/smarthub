<script setup lang="ts">
import { tv } from 'tailwind-variants'

const props = defineProps<{
  label: string
  to: string
  size: 'md' | 'lg'
}>()

const navLink = tv({
  base: 'font-display text-white hover:underline',
  variants: {
    size: {
      md: 'text-[20px] leading-[24px]',
      lg: 'text-[26px] leading-[28px]',
    },
  },
})
</script>

<template>
  <li>
    <NuxtLink
      :class="navLink({ size: props.size })"
      :to="props.to"
    >
      {{ props.label }}
    </NuxtLink>
  </li>
</template>
