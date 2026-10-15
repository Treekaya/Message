<template>

  <section class="relative overflow-hidden bg-blue-950 text-white">

    <!-- große dekorative Formen -->
    <div
      class="pointer-events-none absolute -left-40 -top-40
             h-125 w-125 rounded-full
             bg-[#6d4aff]/25"
    ></div>

    <div
      class="pointer-events-none absolute -bottom-56 -right-40
             h-150 w-150 rounded-full
             bg-[#EED9C4]/10"
    ></div>


    <BaseContent class="relative py-28 sm:py-36">


      <!-- GESCHICHTE -->

      <div
        class="relative mx-auto mt-20 max-w-5xl"
      >

        <!-- verbindende Linie -->
        <div
          class="absolute left-1/2 top-0 hidden h-full
                 w-px -translate-x-1/2
                 bg-white/10 md:block"
        ></div>


        <!-- SZENE 1 -->

        <div
          class="relative grid items-center gap-12
                 md:grid-cols-2 md:gap-20"
        >

          <!-- Elefant -->
          <div class="relative flex justify-center">

            <!-- beige Bühne -->
            <div
              class="absolute h-72 w-72 rounded-full
                     bg-[#EED9C4]/20
                     sm:h-80 sm:w-80"
            ></div>

            <!-- lila kleiner Akzent -->
            <div
              class="absolute -right-3 top-10 h-16 w-16
                     rounded-full bg-[#6d4aff]/70"
            ></div>

            <img
              src="/img/Olifant.png"
              alt="Ein Elefant an einer Kette"
              class="relative mt-12 z-10 w-64 drop-shadow-2xl
                     sm:w-80"
            />

          </div>


          <!-- Text -->
          <div class="relative">

            <p
              class="-mt-4 font-serif text-2xl leading-relaxed
                     text-white sm:text-3xl"
            >
              Ein Mädchen fragt:
            </p>

            <p
              class="mt-5 border-l-2 border-[#6d4aff]
                     pl-6 text-xl italic leading-9 text-blue-100"
            >
              „Warum befreit sich dieser große, starke, erwachsene
              Elefant nicht von seiner Kette?“
            </p>

          </div>

        </div>


        <!-- SZENE 2 -->

        <div
          class="relative mt-24 grid items-center gap-12
                 md:grid-cols-2 md:gap-20"
        >

          <!-- leerer Raum links -->
          <div
            class="hidden md:block"
          ></div>


          <!-- Antwort -->
          <div class="relative">

            <p
              class="-mt-4 text-lg leading-8 text-blue-100/70"
            >
              Nachdem zahlreiche Erwachsene keine Antwort wussten,
              sagt einer:
            </p>

            <div
              class="mt-8 border-l-2 border-[#EED9C4]/60
                     pl-6"
            >

              <p
                class="font-serif text-2xl leading-relaxed
                       text-[#EED9C4] sm:text-3xl"
              >
                „Weißt du … als Kind konnte er es nicht
                und als Erwachsener hat er es nie wieder versucht.“
              </p>

            </div>

          </div>

        </div>


        <!-- ÜBERLEITUNG -->

        <div
          class="relative mt-28 text-center"
        >

          <div
            class="mx-auto h-px w-16 bg-[#6d4aff]"
          ></div>

          <p
            class="mx-auto mt-10 max-w-2xl font-serif
                   text-2xl leading-relaxed text-white
                   sm:text-3xl"
          >
            Manchmal tragen wir Dinge mit uns,
            die einmal wahr waren –
            <span class="text-[#EED9C4]">
              aber heute nicht mehr sein müssen.
            </span>
          </p>

        </div>


        <!-- ABSCHLUSS -->

        <div
          class="mt-20 text-center"
        >

          <a
            href="/angebot"
            class="mt-8 inline-flex items-center gap-3
                   rounded-full bg-[#EED9C4] px-7 py-3.5
                   text-sm font-semibold text-blue-950
                   transition hover:bg-white"
          >
           Termin buchen
            <span>→</span>
          </a>

        </div>

      </div>

    </BaseContent>

  </section>

</template>