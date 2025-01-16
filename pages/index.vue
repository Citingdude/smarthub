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
    <section class="pt-11 pb-20">
      <div class="container bg-white pt-16 pb-20 pl-20 pr-16">
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
