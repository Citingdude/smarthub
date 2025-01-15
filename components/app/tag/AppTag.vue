<script setup lang="ts">
const props = defineProps<{
  label: string
}>()
</script>

<template>
  <div class="bg-white py-[5px] px-[7px] w-fit">
    <p class="text-[12px] leading-[16px] font-body lowercase">
      {{ props.label }}
    </p>
  </div>
</template>
