<script setup lang="ts">
import { tv } from 'tailwind-variants'

const props = defineProps<{
  label: string
  to: string
  color: 'primary' | 'white'
  border?: 'white' | 'grey'
}>()

const button = tv({
  slots: {
    base: 'py-[14px] px-5 font-bold font-display text-lg rounded-full transition flex items-center gap-[10px] w-full sm:w-fit group',
    icon: '',
  },
  base: 'py-[14px] px-5 font-bold font-display text-lg rounded-full transition flex items-center gap-[10px] w-full sm:w-fit',
  variants: {
    color: {
      white: {
        base: 'bg-white hover:bg-gradient-to-r hover:from-gradient-from hover:to-gradient-to text-dark fill-primary hover:fill-white hover:text-white',
        icon: 'fill-dark group-hover:fill-white',
      },
      primary: {
        base: 'bg-gradient-to-r from-gradient-from to-gradient-to text-white hover:brightness-90',
        icon: 'fill-white',
      },
    },
    border: {
      white: {
        base: 'border border-white',
      },
      grey: {
        base: 'border border-[#C1C1C1]',
      },
    },
  },
})

const {
  base,
  icon,
} = button({
  color: props.color,
  border: props.border,
})
</script>

<template>
  <NuxtLink
    :to="props.to"
    :class="base()"
  >
    <span>
      {{ props.label }}
    </span>

    <IconArrowRight :class="icon()" />
  </NuxtLink>
</template>
