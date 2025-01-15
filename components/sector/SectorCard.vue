<script setup lang="ts">
const props = defineProps<{
  icon: 'food' | 'health' | 'creativity' | 'logistics' | 'cleantech'
  hasDivider?: boolean
  label: string
}>()
</script>

<template>
  <NuxtLink
    class="flex flex-col items-center border-black/20 hover:bg-primary/10 p-4 transition" to="/"
    :class="{ 'border-r': props.hasDivider }"
  >
    <div class="size-16">
      <img
        v-if="props.icon === 'food'"
        class="object-contain"
        src="/images/sector/food.png"
        alt="Food"
      >
      <img
        v-else-if="props.icon === 'health'"
        class="object-contain"
        src="/images/sector/health.png"
        alt="Health"
      >
      <img
        v-else-if="props.icon === 'creativity'"
        class="object-contain"
        src="/images/sector/creativity.png"
        alt="Creativity"
      >
      <img
        v-else-if="props.icon === 'logistics'"
        class="object-contain"
        src="/images/sector/logistics.png"
        alt="Health"
      >
      <img
        v-else-if="props.icon === 'cleantech'"
        class="object-contain"
        src="/images/sector/cleantech.png"
        alt="Health"
      >
    </div>
    <!-- <SectorIconFood v-if="props.icon === 'food'" />
    <SectorIconHealth v-if="props.icon === 'health'" />
    <SectorIconCreativity v-if="props.icon === 'creativity'" />
    <SectorIconLogistics v-if="props.icon === 'logistics'" />
    <SectorIconCleantech v-if="props.icon === 'cleantech'" /> -->

    <h3 class="flex items-center gap-2 mt-8">
      <span class="text-lg underline font-bold">
        {{ label }}
      </span>

      <IconArrowRight class="fill-primary" />
    </h3>
  </NuxtLink>
</template>
