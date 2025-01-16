<template>
  <section class="bg-gradient-to-r from-gradient-from to-gradient-to pb-20">
    <div class="container">
      <AppLogo class="translate-y-[-36%]" />

      <div class="flex flex-wrap justify-between gap-16">
        <div class="flex flex-col gap-8 max-w-72 pt-8">
          <div>
            <h2 class="text-[22px] leading-[26px] font-bold text-white font-display">
              Kennisregio Vlaams-Brabant
            </h2>

            <p class="text font-display text-[20px] leading-[26px] text-white mt-4">
              Kennisregio Vlaams-Brabant
              Een unieke concentratie van kennisinstellingen en -bedrijven, in het hart van Europa.
            </p>
          </div>

          <div>
            <h3 class="text-[18px] leading-[24px] font-bold text-white font-display">
              Algemene vragen
            </h3>

            <div class="mt-4 flex flex-col gap-1">
              <a
                href="mailto:info@smarthubvlaamsbrabant.be"
                class="flex items-center gap-2 underline text-white hover:no-underline"
              >
                <IconMail />
                <p class="font-display text-[18px] leading-[24px]">
                  info@smarthubvlaamsbrabant.be
                </p>
              </a>

              <a
                href="tel:+32 (0)16 12 30 00"
                class="flex items-center gap-2 text-white underline hover:no-underline"
              >
                <IconPhone />
                <p class="font-display text-[18px] leading-[24px]">
                  +32 (0)16 12 30 00
                </p>
              </a>
            </div>
          </div>

          <div>
            <h3 class="text-[18px] leading-[24px] font-bold text-white font-display">
              Volg ons via
            </h3>

            <div class="mt-4 flex gap-4 items-center">
              <IconFacebook />
              <IconInstagram />
              <IconLinkedin />
              <IconYoutube />
            </div>
          </div>
        </div>

        <AppFooterMainNav />

        <form class="bg-white p-10" action="">
          <h3 class="text-[30px] leading-[36px] font-display max-w-56">
            Schrijf je in op onze nieuwsbrief
          </h3>

          <p class="max-w-[350px] mt-4">
            Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.
          </p>

          <div class="flex flex-col mt-8 gap-2 max-w-80">
            <label class="font-bold font-display" for="email">
              Email
            </label>

            <input
              id="email"
              type="email"
              placeholder="Email"
              class="py-2 px-5 border border-dark"
            >
          </div>

          <div class="flex items-start gap-2 mt-6 max-w-80">
            <input
              id="privacy"
              type="checkbox"
              placeholder="Email"
              class="size-8"
            >

            <label class="font-light" for="privacy">
              Ik verklaar dat ik de <a class="underline" href="/">privacy policy</a> heb gelezen en goedgekeurd.
            </label>
          </div>

          <AppButton class="mt-6" label="Inschrijven" to="/" color="primary" />
        </form>
      </div>
    </div>
  </section>
</template>
