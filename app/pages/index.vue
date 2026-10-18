<template>

  <div class="overflow-hidden -mt-10">

    <section class="relative bg-[#faf8f4]">

      <!-- dekorativer lila Kreis -->
      <div
        class="pointer-events-none absolute -right-32 -top-32
               h-96 w-96 rounded-full bg-[#6d4aff]/8"
      ></div>

      <BaseContent class="relative py-20 sm:py-28 lg:py-32">

        <div class="grid items-center gab-2 lg:grid-cols-[1fr_440px]">

          <!-- TEXT -->
          <div class="relative z-10">

            <span
              class="inline-flex items-center gap-3
                     text-sm font-semibold uppercase tracking-[0.25em]
                     text-[#6d4aff]"
            >
              <span class="h-px w-8 bg-[#6d4aff]"></span>
              Psychosoziale Beratung
            </span>

            <h1
              class="mt-7 max-w-3xl font-serif text-6xl
                     leading-[0.88] tracking-tight text-blue-950
                     sm:text-7xl lg:text-8xl"
            >
              Vom Überleben

              <span
                class="block pl-8 pt-3 italic text-blue-950/65
                       sm:pl-20"
              >
                zum Leben.
              </span>
            </h1>

            <p
              class="mt-10 max-w-xl text-xl leading-9 text-slate-600"
            >
              Ich heiße Ingrid Köck. Ich begleite Menschen durch schwierige Zeiten und unterstütze Sie dabei, wieder im
              Leben Fuß zu fassen.
            </p>

            <div class="mt-10 flex flex-wrap items-center gap-6">

              <a
                href="/ueber-mich"
                class="group inline-flex items-center gap-3
                       rounded-full bg-blue-950 px-7 py-3.5
                       text-sm font-medium text-white
                       transition hover:bg-[#6d4aff]"
              >
                Mehr über mich
                <span
                  class="transition-transform group-hover:translate-x-1"
                >
                  →
                </span>
              </a>

              <a
                href="/angebot"
                class="text-sm font-medium text-blue-950
                       underline decoration-[#6d4aff]/40
                       underline-offset-8
                       transition hover:text-[#6d4aff]"
              >
                Wobei ich Sie begleiten kann
              </a>

            </div>

          </div>


          <!-- FOTO -->
          <div
            class="relative mx-auto w-full max-w-md"
          >

            <!-- lila Akzent dahinter -->
            <div
              class="absolute -right-5 -top-5 h-full w-full
                     bg-[#6d4aff]/15"
            ></div>

            <!-- beige Schattenform -->
            <div
              class="absolute -bottom-5 -left-5 h-full w-full
                     bg-[#EED9C4]"
            ></div>

            <!-- Foto -->
            <div
              class="relative bg-white p-4
                     shadow-[0_25px_60px_rgba(23,37,84,0.16)]"
            >

              <img
                src="/img/Ingrid.jpg"
                alt="Ingrid, psychologische Beraterin"
                class=" aspect-3/4 w-full object-cover"
              />

              <div
                class="absolute bottom-7 left-7
                       bg-blue-950 px-5 py-3 text-white"
              >
                <p class="font-serif text-xl">
                  Ingrid Köck
                </p>

                <p
                  class="mt-0.5 text-[10px] uppercase
                         tracking-[0.2em] text-blue-100"
                >
                  Beratung & Begleitung
                </p>
              </div>

            </div>

          </div>

        </div>

      </BaseContent>

    </section>


    <SectionKennstDuDass />

    <SectionElifant />

  </div>

</template>
