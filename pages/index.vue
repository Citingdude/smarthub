<template>
  <main class="bg-light">
    <!-- Hero -->
    <section class="py-12 sm:py-24 lg:py-56 xl:py-[275px] relative overflow-hidden">
      <img class="w-full absolute inset-0" src="/images/hero.jpg" alt="">
      <div class="container relative">
        <div class="max-w-[600px] flex flex-col gap-[15px]">
          <TextH1 class="text-white">
            Vandaag innoveren voor morgen.
          </TextH1>

          <p class="text-[14px] leading-[15px] sm:text-[28px] sm:leading-[30px] text-white">
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
        <AppBanner class=" lg:mt-[-8rem]" />
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
        </div>

        <ProjectSlider class="w-full mt-10" />
      </div>
    </section>

    <!-- Sectors -->
    <section class="pt-11 pb-20 ">
      <div class="relative container bg-white pt-16 pb-20 pl-20 pr-16">
        <svg class="absolute bottom-0 right-0 scale-50 sm:scale-100 origin-bottom-right" width="621" height="576" viewBox="0 0 621 576" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path opacity="0.04" d="M701.432 363.957L689.88 250.575C688.311 236.028 675.19 225.331 660.643 226.758L513.317 242.018C498.77 243.444 491.639 233.746 497.629 220.34L558.242 85.1366C564.232 71.7304 558.242 55.8997 544.836 49.9097L440.724 3.27315C427.318 -2.71685 411.487 3.27315 405.497 16.6794L344.884 151.74C338.894 165.146 327.056 166.43 318.499 154.45L231.644 34.3642C223.087 22.5268 206.258 19.817 194.42 28.5168L102.146 95.2626C90.3084 103.962 87.5987 120.649 96.1558 132.486L183.011 252.572C191.568 264.409 186.719 275.391 172.029 276.96L24.7036 292.077C10.1564 293.503 -0.682663 306.624 0.886149 321.314L12.4383 434.554C14.0071 449.244 27.1281 459.94 41.6753 458.371L189.001 443.254C203.548 441.685 210.536 451.526 204.546 464.789L143.933 599.85C137.943 613.256 143.933 629.086 157.339 634.934L261.309 681.57C274.715 687.56 290.546 681.57 296.536 668.164L357.149 533.104C363.139 519.698 374.976 518.557 383.534 530.394L470.389 650.479C478.946 662.459 495.632 665.027 507.612 656.469L600.03 589.581C611.867 581.024 614.577 564.337 606.02 552.5L519.164 432.415C510.607 420.435 515.456 409.453 530.146 408.027L677.472 392.909C692.162 391.34 702.858 378.219 701.289 363.672" fill="#0E0F0E" />
        </svg>

        <div class="relative">
          <TextSubtitle>
            Sectoren
          </TextSubtitle>

          <TextH2 class="mt-2">
            Donec id elit non mi porta
          </TextH2>

          <TextBody class="mt-4 max-w-4xl">
            Nullam id dolor id nibh ultricies vehicula ut id elit. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Nullam id dolor id nibh ultricies vehicula ut id elit. Sed posuere consectetur est at lobortis. Lorem ipsum dolor sit amet, consectetur adipiscing elit.
          </TextBody>

          <div class="grid sm:grid-cols-2 lg:grid-cols-5 mt-16">
            <SectorCard
              icon="food"
              has-divider
              label="Food"
            />
            <SectorCard
              icon="health"
              has-divider
              label="Health"
            />
            <SectorCard
              icon="creativity"
              has-divider
              label="Creativity"
            />
            <SectorCard
              has-divider
              icon="logistics"
              label="Logistics"
            />
            <SectorCard
              icon="cleantech"
              label="Cleantech"
            />
          </div>

          <AppButton
            class="mt-11"
            to="/"
            label="Ontdek meer over de sectoren"
            color="white"
            border="grey"
          />
        </div>
      </div>
    </section>

    <!-- Kpi's -->
    <section class="bg-white py-28">
      <div class="container">
        <div class="max-w-2xl">
          <TextSubtitle>
            In cijfers
          </TextSubtitle>

          <TextH2 class="mt-2">
            Praesent commodo cursus magna
          </TextH2>

          <TextBody class="mt-4">
            Onze impact integer posuere erat a ante venenatis dapibus posuere velit aliquet. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Maecenas faucibus mollis interdum.
          </TextBody>
        </div>

        <KpiGrid class="mt-11" />
      </div>
    </section>

    <!-- Events -->
    <section class="py-28">
      <div class="container">
        <TextSubtitle>
          Agenda
        </TextSubtitle>

        <div class="flex items-center gap-6">
          <TextH3>
            Binnenkort
          </TextH3>

          <AppDividerVertical />

          <AppLink to="/" label="Bekijk alle evenementen" />
        </div>

        <div class="grid xl:grid-cols-2 gap-6 mt-11">
          <EventCard
            :image="{
              src: '/images/event/event_2.jpg',
              alt: 'Ai',
            }"
            title="Design for Innovation - Learn & Match"
            date="04/03/2023"
            location="Leuven"
            :tags="[
              {
                color: 'orange',
                label: 'Laatste tickets',
              },
              {
                color: 'red',
                label: 'Uitverkocht',
              },
              {
                color: 'grey',
                label: 'Conference',
              },
            ]"
          />
          <EventCard
            :image="{
              src: '/images/event/event.jpg',
              alt: 'Ai',
            }"
            title="Future generation conference"
            date="04/03/2023"
            location="Leuven"
            :tags="[
              {
                color: 'grey',
                label: 'Conference',
              },
            ]"
          />
        </div>
      </div>
    </section>

    <!-- News -->
    <section class="bg-white py-32 overflow-hidden">
      <div class="container">
        <TextSubtitle>
          Nieuws
        </TextSubtitle>

        <div class="flex items-center gap-6">
          <TextH3>
            Actueel
          </TextH3>

          <AppDividerVertical />

          <AppLink to="/" label="Bekijk alle nieuws" />
        </div>

        <div class="mt-8 flex flex-col xl:flex-row gap-6 xl:min-w-[120%]">
          <NewsCard />
          <NewsCard />
        </div>
      </div>
    </section>
  </main>
</template>
