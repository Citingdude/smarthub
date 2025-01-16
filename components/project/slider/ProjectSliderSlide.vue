<template>
  <NuxtLink
    to="/"
    class="relative group/project-slide"
  >
    <div>
      <img
        class="w-full h-auto object-cover"
        src="/images/project/project_image.jpg"
        alt="Project"
      >
      <div class="opacity-0 group-hover/project-slide:opacity-100 absolute z-10 bg-black/60 inset-0 transition" />
    </div>

    <div class="absolute z-10 bottom-0 left-0 p-5 sm:pb-12 sm:px-10">
      <AppTag label="Cleantech" />

      <h3 class="text-[20px] leading-tight sm:text-[35px] sm:leading-[40px] font-display text-white mt-7">
        Lorem ipsum dolor sit amet
      </h3>

      <div class="hidden mt-4 group-hover/project-slide:block">
        <p class="text-white font-light text-[20px] leading-[26px]">
          KU Leuven en ingenieursbureau Comate ontwikkelen een innovatieve technologie waarbij een patiënt thuis, op een gebruiksvriendelijke en pijnloze manier, zelf een bloedstaal kan afnemen via een vingerprik.
        </p>

        <AppLink
          class="mt-4"
          label="Meer lezen"
          to="/"
          color="light"
        />
      </div>
    </div>
  </NuxtLink>
</template>
