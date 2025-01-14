<script setup lang="ts">
type Locale = 'nl' | 'en'

const isOpen = ref(false)
const activeLocale = ref<Locale>('nl')

function setLocale(locale: Locale) {
  activeLocale.value = locale
  isOpen.value = false
}
</script>

<template>
  <div class="relative">
    <button @click="isOpen = !isOpen" class="flex items-center gap-2">
      <span class="uppercase font-bold font-display">
        {{ activeLocale }}
      </span>

      <IconChevronDown />
    </button>

    <TransitionSlideIn>
      <div class="absolute top-full left-0 bg-white w-full px-2 py-1" v-if="isOpen">
        <ul>
          <li v-if="activeLocale !== 'en'"  class="uppercase font-bold font-display">
            <button @click="setLocale('en')">
              EN
            </button>
          </li>
          <li v-if="activeLocale !== 'nl'"  class="uppercase font-bold font-display">
            <button @click="setLocale('nl')">
              NL
            </button>
          </li>
        </ul>
      </div>
    </TransitionSlideIn>

  </div>
</template>