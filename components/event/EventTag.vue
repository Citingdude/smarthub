<script setup lang="ts">
import { tv, type VariantProps } from 'tailwind-variants'

type EventTagVariants = VariantProps<typeof eventTag>

export interface EventTagProps {
  label: string
  color: EventTagVariants['color']
}

const props = defineProps<EventTagProps>()

const eventTag = tv({
  base: 'p-[5px] text-[12px] leading-[16px] font-semibold rounded-[4px] w-fit',
  variants: {
    color: {
      orange: 'bg-[#D38218] text-white',
      red: 'bg-primary text-white',
      grey: 'bg-light text-dark',
    },
  },
})
</script>

<template>
  <p :class="eventTag({ color: props.color })">
    {{ label }}
  </p>
</template>
