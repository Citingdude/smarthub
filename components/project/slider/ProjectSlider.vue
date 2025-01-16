<script scrip setup>
import { useKeenSlider } from 'keen-slider/vue'

const [container, slider] = useKeenSlider({
  breakpoints: {
    '(min-width: 1024px)': {
      slides: {
        perView: 3,
        spacing: 20,
      },
    },
  },
  loop: true,
  slides: {
    perView: 2,
    spacing: 10,
  },
})
</script>

<template>
  <div>
    <div class="flex gap-12 sm:justify-end">
      <button
        class="hover:bg-primary/5 rounded-full p-1 transition active:bg-primary/10"
        @click="slider.prev()"
      >
        <IconArrowLeft class="fill-primary size-5" @click="slider.next()" />
      </button>

      <button
        class="hover:bg-primary/5 rounded-full p-1 transition active:bg-primary/10"
        @click="slider.next()"
      >
        <IconArrowRight class="fill-primary size-5" />
      </button>
    </div>

    <div ref="container" class="keen-slider mt-10">
      <div class="keen-slider__slide">
        <ProjectSliderSlide />
      </div>
      <div class="keen-slider__slide">
        <ProjectSliderSlide />
      </div>
      <div class="keen-slider__slide">
        <ProjectSliderSlide />
      </div>
      <div class="keen-slider__slide">
        <ProjectSliderSlide />
      </div>
      <div class="keen-slider__slide">
        <ProjectSliderSlide />
      </div>
    </div>
  </div>
</template>

<style>
  @import url('keen-slider/keen-slider.css');
</style>
