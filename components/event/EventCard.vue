<script setup lang="ts">
import type { EventTagProps } from './EventTag.vue'

const props = defineProps<{
  image: {
    src: string
    alt: string
  }
  title: string
  tags: EventTagProps[]
  date: string
  location: string
}>()
</script>

<template>
  <NuxtLink to="/" class="flex flex-col sm:flex-row">
    <img :src="props.image.src" :alt="props.image.alt">

    <div class="bg-white pt-8 pl-8 pb-7 pr-7 flex flex-col gap-4">
      <div class="flex gap-3">
        <EventTag
          v-for="tag in props.tags"
          :key="tag.label"
          :color="tag.color"
          :label="tag.label"
        />
      </div>

      <h3 class="text-[28px] leading-[33px] font-display">
        {{ props.title }}
      </h3>

      <div class="flex items-center gap-4">
        <div class="flex items-center gap-2">
          <IconCalendar />
          <p class="text-[12px] leading-[28px]">
            {{ props.date }}
          </p>
        </div>

        <div class="flex items-center gap-2">
          <IconLocation />
          <p class="text-[12px] leading-[28px]">
            {{ props.location }}
          </p>
        </div>
      </div>
    </div>
  </NuxtLink>
</template>
