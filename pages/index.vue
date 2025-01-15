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

          <TextBody class="text-[28px] leading-[30px] text-white">
            Smart Hub investeert in slimme projecten, verbindt partners en opent deuren in het buitenland.
          </TextBody>
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
    <section class="relative">
      <div class="container">
        <AppBanner class="-translate-y-32" />
      </div>
    </section>
  </main>
</template>
