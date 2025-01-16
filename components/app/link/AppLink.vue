<script setup lang="ts">
import { tv } from 'tailwind-variants'

const props = withDefaults(defineProps<{
  to: string
  label: string
  color?: 'light' | 'dark'
}>(), {
  color: 'dark',
})

const appLink = tv({
  slots: {
    base: 'flex w-fit gap-2 items-center group',
    text: 'text-lg font-display group-hover:underline transition',
    icon: '',
  },
  variants: {
    color: {
      dark: {
        text: 'group-hover:text-secondary text-dark',
        icon: 'fill-primary',
      },
      light: {
        text: 'text-white',
        icon: 'fill-white',
      },
    },
  },
})

const {
  base,
  text,
  icon,
} = appLink({
  color: props.color,
})
</script>

<template>
  <NuxtLink :class="base()" :to="props.to">
    <span :class="text()">
      {{ label }}
    </span>

    <IconArrowRight :class="icon()" />
  </NuxtLink>
</template>
