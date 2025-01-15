<template>
  <main class="bg-light">
    <!-- Hero -->
    <section class="py-[275px] relative overflow-hidden">
      <img class="w-full absolute inset-0" src="/images/hero.jpg" alt="">
      <div class="container relative">
        <div class="max-w-[600px] flex flex-col gap-[15px]">
          <TextH1 class="text-white">
            Vandaag innoveren voor morgen.
          </TextH1>

          <p class="text-[28px] leading-[30px] text-white">
            Smart Hub investeert in slimme projecten, verbindt partners en opent deuren in het buitenland.
          </p>
        </div>

        <AppButton
          class="mt-10"
          label="Ontdek hoe wij kunnen helpen"
          to="/"
          color="primary"
        />
      </div>
    </section>

    <!-- Banner -->
    <section class="relative pb-11">
      <div class="container">
        <AppBanner class=" mt-[-8rem]" />
      </div>
    </section>

    <!-- Projects -->
    <section class="py-11">
      <div class="container">
        <div class="flex flex-col max-w-3xl">
          <TextSubtitle>
            In de kijker
          </TextSubtitle>

          <TextH2 class="mt-2">
            Leer meer over onze projecten
          </TextH2>

          <TextBody class="mt-4">
            We ondersteunen projecten in <a href="/">Food</a>, <a href="/">Health</a>, <a href="/">Creativity</a>, <a href="/">Logistics</a> & <a href="/">Cleantech</a> Lorem justo odio, dapibus ac facilisis in, egestas eget quam. Maecenas faucibus mollis interdum.
          </TextBody>

          <AppLink
            to="/"
            label="Alle projecten"
            class="mt-4"
          />

          <ProjectSlider class="w-full mt-10" />
        </div>
      </div>
    </section>
  </main>
</template>
