<script scrip setup>
import { useKeenSlider } from 'keen-slider/vue'

const [container] = useKeenSlider({
  breakpoints: {
    '(min-width: 1024px)': {
      slides: {
        perView: 3,
        spacing: 20,
      },
    },
  },
  slides: {
    perView: 2,
    spacing: 10,
  },
})
</script>

<template>
  <div ref="container" class="keen-slider">
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
</template>

<style>
  @import url('keen-slider/keen-slider.css');
</style>
