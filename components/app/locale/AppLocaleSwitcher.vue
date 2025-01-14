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
    <button class="flex items-center gap-2" @click="isOpen = !isOpen">
      <span class="uppercase font-bold font-display">
        {{ activeLocale }}
      </span>

      <IconChevronDown />
    </button>

    <TransitionSlideIn>
      <div v-if="isOpen" class="absolute top-full left-0 bg-white w-full px-2 py-1">
        <ul>
          <li v-if="activeLocale !== 'en'" class="uppercase font-bold font-display">
            <button @click="setLocale('en')">
              EN
            </button>
          </li>
          <li v-if="activeLocale !== 'nl'" class="uppercase font-bold font-display">
            <button @click="setLocale('nl')">
              NL
            </button>
          </li>
        </ul>
      </div>
    </TransitionSlideIn>
  </div>
</template>
