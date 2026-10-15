<template>

  <div class="-mt-16">

    <!-- ÜBERSCHRIFT -->
    <section class="pt-16 bg-[#faf8f4]">
      <BaseContent class="py-16 sm:py-20">

        <div class="mx-auto max-w-3xl text-center">

          <span class="text-sm font-medium uppercase tracking-[0.3em] text-[#806b53]">
            Kontakt & Termine
          </span>

          <h1 class="mt-5 font-serif text-5xl font-medium text-stone-800 sm:text-6xl">
            Ich freue mich auf Sie
          </h1>

          <div class="mx-auto mt-7 h-px w-20 bg-[#9a8367]/60"></div>

        </div>

      </BaseContent>
    </section>


    <!-- EINBLICK IN DEN RAUM --> 
     <section class="bg-[#faf8f4]"> 
      <BaseContent class="pb-16 sm:pb-20"> 
        <div class="mx-auto max-w-5xl"> 
          <img 
            src="/img/Raum.jpg" 
            alt="Einblick in den Raum" 
            class="h-72 w-full rounded-3xl object-cover shadow-sm sm:h-96 lg:h-115" /> 
        </div> 
      </BaseContent> 
    </section>


    <!-- KONTAKT -->
    <section class="bg-[#faf8f4]">
      <BaseContent class="pb-24 sm:pb-28">

        <div class="mx-auto max-w-5xl">

          <div
            class="flex flex-col gap-0 overflow-hidden
                   rounded-3xl shadow-sm ring-1 ring-[#d8cdbd]
                   md:flex-row"
          >

            <!-- Kontaktkarte -->
            <div class="min-w-80 space-y-8 bg-white p-8 sm:p-10">

              <div class="relative">
                <LucideMail
                  :stroke-width="2"
                  :size="28"
                  class="absolute -rotate-3"
                  color="#806b53"
                />
                <div class="ml-10">
                  <p class="text-xs font-semibold uppercase tracking-[0.2em] text-[#9a8367]">
                    Email
                  </p>
                  <a
                    href="mailto:ingrid.koeck@gmx.at"
                    class="mt-1 block font-medium text-stone-800
                           transition hover:text-[#806b53]"
                  >
                    ingrid.koeck@gmx.at
                  </a>
                </div>
              </div>

              <div class="relative">
                <LucideMapPin
                  :stroke-width="2"
                  :size="28"
                  class="absolute -rotate-3"
                  color="#806b53"
                />
                <div class="ml-10">
                  <p class="text-xs font-semibold uppercase tracking-[0.2em] text-[#9a8367]">
                    Adresse
                  </p>
                  <p class="mt-1 leading-7 text-stone-800">
                    Landstrasse 59 – 61<br />
                    A-4020 Linz<br />
                    0680 – 216 46 16
                  </p>
                </div>
              </div>

              <div class="relative">
                <LucideClock
                  :stroke-width="2"
                  :size="28"
                  class="absolute -rotate-3"
                  color="#806b53"
                />
                <div class="ml-10">
                  <p class="text-xs font-semibold uppercase tracking-[0.2em] text-[#9a8367]">
                    Öffnungszeiten
                  </p>
                  <p class="mt-1 leading-7 text-stone-800">
                    Nach Vereinbarung<br />
                    <span class="text-stone-500">
                      Bitte vorher Termin absprechen
                    </span>
                  </p>
                </div>
              </div>

            </div>

            <!-- Karte (statisch statt iframe) -->
            <div class="relative w-full">
              <img
                src="/img/Karte.png"
                alt="Standortkarte von Massagepraxis Ingrid Köck in Linz"
                class="h-75 w-full border-l-0 md:h-auto md:min-h-100"
              />
              <div
                class="absolute bottom-2 left-2 right-2 rounded-md bg-black/60 px-3 py-2 text-xs text-white backdrop-blur-sm"
              >
                <span class="block font-medium">Karte:</span>
                <a
                  href="https://www.openstreetmap.org"
                  target="_blank"
                  rel="noopener noreferrer"
                  class="text-stone-200 underline hover:text-white"
                >
                  OpenStreetMap-Mitwirkende
                </a>
              </div>
            </div>

          </div>
        </div>

      </BaseContent>
    </section>


    <!-- KOSTEN -->
    <section class="bg-[#eee7dc]">

      <BaseContent class="py-24 sm:py-28">

        <div class="mx-auto max-w-5xl">
          <div class="mb-14 max-w-3xl">

            <span class="text-sm font-medium uppercase tracking-[0.3em] text-[#806b53]">
              Gut zu wissen
            </span>

            <h2 class="mt-4 font-serif text-4xl text-stone-800 sm:text-5xl">
              Rückerstattung der Kosten
            </h2>

            <p class="mt-6 text-lg leading-8 text-stone-600">
              Die Möglichkeiten einer Kostenrückerstattung können je nach
              Versicherung und persönlicher Situation unterschiedlich sein.
            </p>

          </div>


          <!-- Gesetzliche Kassen -->
          <div class="border-t border-[#cfc0ac] py-9">
            <div class="grid gap-5 md:grid-cols-[180px_1fr]">

              <span class="text-xs font-semibold uppercase tracking-[0.2em] text-[#9a8367]">
                Gesetzlich
              </span>

              <div>

                <h3 class="font-serif text-2xl text-stone-800">
                  Gesetzliche Krankenkassen
                </h3>

                <p class="mt-4 max-w-3xl leading-8 text-stone-600">
                  Der Großteil der gesetzlichen Krankenkassen in Österreich
                  sieht keine Rückerstattung des Honorars für diverse Massagen
                  und Coaching vor.
                </p>

              </div>

            </div>

          </div>


          <!-- SVS -->
          <div class="border-t border-[#cfc0ac] py-9">
            <div class="grid gap-5 md:grid-cols-[180px_1fr]">

              <span class="text-xs font-semibold uppercase tracking-[0.2em] text-[#9a8367]">
                SVS
              </span>

              <div>

                <h3 class="font-serif text-2xl text-stone-800">
                  Selbstständige & Bauern
                </h3>

                <p class="mt-4 max-w-3xl leading-8 text-stone-600">
                  Einmal pro Kalenderjahr können SVS-Versicherte den
                  sogenannten „Gesundheitshunderter" einlösen.
                  Für einige gesundheitsfördernde Maßnahmen zahlt die
                  SVS € 100,00.
                </p>

                <a
                  href="https://www.svs.at"
                  target="_blank"
                  rel="noopener noreferrer"
                  class="mt-5 inline-flex items-center gap-2
                         font-medium text-[#806b53]
                         transition hover:gap-3"
                >
                  Mehr zum Gesundheitshunderter
                  <span aria-hidden="true">→</span>
                </a>

              </div>
            </div>
          </div>


          <!-- Private Versicherung -->
          <div class="border-y border-[#cfc0ac] py-9">
            <div class="grid gap-5 md:grid-cols-[180px_1fr]">

              <span class="text-xs font-semibold uppercase tracking-[0.2em] text-[#9a8367]">
                Privat
              </span>

              <div>

                <h3 class="font-serif text-2xl text-stone-800">
                  Private Krankenversicherung
                </h3>

                <p class="mt-4 max-w-3xl leading-8 text-stone-600">
                  Bei Abschluss mancher privater Zusatz-Krankenversicherungen
                  könnte die Versicherung das gesamte oder Teile des Coachings
                  beziehungsweise der Massagen übernehmen.
                </p>

                <p class="mt-4 font-medium text-stone-700">
                  Bitte erkundigen Sie sich direkt bei Ihrer Versicherung,
                  ob und in welchem Umfang eine Kostenübernahme möglich ist.
                </p>

              </div>
            </div>
          </div>
        </div>
      </BaseContent>
    </section>

    <!-- LSB BERUFSPROFIL -->
    <section class="bg-blue-300">
      <BaseContent class="py-20 sm:py-24">

        <div class="mx-auto max-w-5xl text-center">

          <span  class="text-sm font-medium uppercase tracking-[0.3em] text-[#806b53]">
            Berufsprofil
          </span>

          <h2 class="mt-4 font-serif text-4xl text-stone-800 sm:text-5xl">
            Lebens- und Sozialberatung
          </h2>

          <div class="mx-auto mt-7 mb-10 h-px w-20 bg-[#9a8367]/60"></div>

          <img
            src="/img/Impuls_pro_CMYK.jpg"
            alt="Offizielles Logo für Lebens- und Sozialberater"
            class="mx-auto h-32 w-auto rounded-xl shadow-sm md:h-40"
          />

        </div>

      </BaseContent>
    </section>

  </div>
</template>