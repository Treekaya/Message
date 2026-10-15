<template>
  <div class="-mt-10 bg-stone-100 text-stone-800">

    <!-- HERO / WALL -->
    <section
      class="relative bg-stone-100 text-stone-800 min-h-162.5 overflow-hidden bg-cover bg-center bg-fixed"
      style="background-image: url('/img/Wallpaper.png')"
    >
      <!-- leichte Abdunklung -->
      <div class="absolute inset-0 bg-black/10"></div>

      <div class="relative mx-auto flex min-h-162.5 max-w-6xl items-center justify-center px-6 py-16">

        <!-- Bilderrahmen -->
        <div class="relative -rotate-1">

          <!-- Schatten -->
          <div
            class="absolute -inset-5 rounded-sm bg-black/30 blur-xl"
          ></div>

          <!-- äußerer Rahmen -->
          <div
            class="relative bg-linear-to-br from-amber-900 via-yellow-800 to-amber-950 p-3 shadow-2xl"
          >

            <!-- innerer Rahmen -->
            <div class="bg-linear-to-br from-stone-700 via-stone-300 to-stone-700 p-2">

              <!-- Passepartout -->
              <div class="bg-[#f5f0e6] p-5 shadow-inner">

                <div class="relative overflow-hidden bg-stone-200">
                  <img
                    src="/img/Ingrid2.jpg"
                    alt="Portrait"
                    class="h-105 object-cover object-center sm:h-120 sm:w-130"
                  />

                  <!-- dezente Spiegelung -->
                  <div
                    class="pointer-events-none absolute inset-0 bg-linear-to-tr from-white/10 via-transparent to-white/20"
                  ></div>
                </div>

                <!-- Beschriftung unter dem Foto -->
                <div class="pt-5 text-center">
                  <p class="font-serif text-2xl tracking-wide text-stone-800">
                    Wer bin ich?
                  </p>

                  <p class="mt-1 text-sm uppercase tracking-[0.25em] text-stone-500">
                    Ingrid Köck
                    dipl. Lebens- und Sozialarbeiterin
                  </p>
                </div>

              </div>
            </div>
          </div>

        </div>
      </div>
    </section>


    <!-- INHALT -->
    <main class="mx-auto max-w-5xl px-6 py-20 sm:px-8">

      <!-- Überschrift -->
      <header class="mb-16 text-center">
        <span
          class="text-sm font-medium uppercase tracking-[0.3em] text-amber-700"
        >
          Persönliches
        </span>

        <h1
          class="mt-4 font-serif text-4xl font-medium text-stone-900 sm:text-5xl"
        >
          Wer bin ich?
        </h1>

        <div class="mx-auto mt-6 h-px w-24 bg-amber-700/50"></div>

        <p
          class="mx-auto mt-6 max-w-2xl text-lg leading-8 text-stone-600"
        >
          Mit wem bekommen Sie es zu tun?
        </p>
      </header>


      <!-- TEXT -->
      <article class="space-y-16">

        <!-- Abschnitt 1 -->
        <section>
          <p class="text-lg leading-9 text-stone-700">
            Aufgewachsen bin ich in der grünen Steiermark und das kann ich von mir
            wirklich behaupten. Als Försterstochter im idyllischen Holzhaus am
            Waldesrand, mit Hund, Katz', Reh und so manch anderem Tier, durfte ich
            sehr naturnah meine Kindheit verbringen.
          </p>

          <p class="mt-6 text-lg leading-9 text-stone-700">
            Bis zu meinem Handelsschulabschluss in Bruck/Mur wollte ich schon immer
            hinaus in die große weite Welt. Es zog mich weg, ich war abenteuerlustig,
            keiner in meiner Familie hatte das so wie ich.
          </p>
        </section>


        <!-- Zitat -->
        <blockquote
          class="border-l-4 border-amber-700 bg-amber-50/70 px-8 py-7 font-serif
                 text-2xl italic leading-relaxed text-stone-700 shadow-sm"
        >
          „Das veränderte mein Leben maßgeblich.“
        </blockquote>


        <!-- Abschnitt 2 -->
        <section>
          <h2 class="font-serif text-3xl text-stone-900">
            Der Weg zu meiner Berufung
          </h2>

          <div class="mt-6 space-y-6 text-lg leading-9 text-stone-700">
            <p>
              Meine erste Station war ein missglückter Versuch als Au-pair-Mädchen
              in London. Das Vorhaben, für ein Jahr zu bleiben, scheiterte kläglich
              an meinem Heimweh und der Anpassung an neue Gegebenheiten.
            </p>

            <p>
              So kam es bereits nach 10 Tagen zu einer vorgezogenen Heimreise.
              In der Not suchten meine Eltern bereits intensiv nach einer
              Ersatzlösung und so fing ich kurz nach meinem Heimkommen mit einem
              Massagekurs in Graz an.
            </p>

            <p>
              Als Masseurin bereicherten zahlreiche Saisongebiete, wunderschöne
              Hotels und viele Gäste aus der ganzen Welt - darunter auch Könige
              und Prinzessinnen - jahrelang meinen Horizont.
            </p>

            <p>
              Menschen berichteten mir aus ihrer inneren und äußeren Welt …
              lustige Geschichten, traurige Geschichten. Alles wurde mir am
              Massagetisch erzählt.
            </p>

            <p class="font-serif text-2xl text-amber-800">
              Ich fand meine Berufung.
            </p>
          </div>
        </section>


        <!-- Timeline / Stationen -->
        <section class="rounded-2xl bg-white p-8 shadow-sm ring-1 ring-stone-200 sm:p-10">

          <h2 class="font-serif text-3xl text-stone-900">
            Meine Lebenslinie
          </h2>

          <div class="mt-8 space-y-8">

            <div class="flex gap-5">
              <div
                class="mt-2 h-3 w-3 shrink-0 rounded-full bg-amber-700 ring-4 ring-amber-100"
              ></div>

              <div>
                <span class="text-sm font-semibold uppercase tracking-widest text-amber-700">
                  Kindberg/Stmk 
                </span>
                <p class="mt-2 leading-8 text-stone-600">
                  geb 1969 in Bruck/Mur, aufgewachsen in Kindberg im Forsthaus, mitten in der Natur
                </p>
              </div>
            </div>

            <div class="flex gap-5">
              <div
                class="mt-2 h-3 w-3 shrink-0 rounded-full bg-amber-700 ring-4 ring-amber-100"
              ></div>

              <div>
                <span class="text-sm font-semibold uppercase tracking-widest text-amber-700">
                  Graz
                </span>
                <p class="mt-2 leading-8 text-stone-600">
                  1987 Beginn meines beruflichen Weges als Masseurin, mit jährlichen Weiterbildungen bis heute 
                </p>
              </div>
            </div>

            <div class="flex gap-5">
              <div
                class="mt-2 h-3 w-3 shrink-0 rounded-full bg-amber-700 ring-4 ring-amber-100"
              ></div>

              <div>
                <span class="text-sm font-semibold uppercase tracking-widest text-amber-700">
                  Linz
                </span>
                <p class="mt-2 leading-8 text-stone-600">
                  1998 Umzug nach Linz. Start meiner Selbständigkeit. Finden einer neuen Heimat durch viele neue Begegnungen mit netten Menschen und mittlerweile einem großen Freundeskreis. 
                </p>
              </div>
            </div>

            <div class="flex gap-5">
              <div
                class="mt-2 h-3 w-3 shrink-0 rounded-full bg-amber-700 ring-4 ring-amber-100"
              ></div>

              <div>
                <span class="text-sm font-semibold uppercase tracking-widest text-amber-700">
                  2023
                </span>
                <p class="mt-2 leading-8 text-stone-600">
                  Start als Lebens- und Sozialberaterin, Coaching, Supervision, Aufstellungsarbeit
                  … eine wunderbare Ergänzung mit der Arbeit für Menschen
                </p>
              </div>
            </div>

            <div class="flex gap-5">
              <div
                class="mt-2 h-3 w-3 shrink-0 rounded-full bg-amber-700 ring-4 ring-amber-100"
              ></div>

              <div>
                <span class="text-sm font-semibold uppercase tracking-widest text-amber-700">
                  Heute
                </span>
                <p class="mt-2 leading-8 text-stone-600">
                  Lebens- und Sozialberatung, Coaching, Supervision und
                  Aufstellungsarbeit.
                </p>
              </div>
            </div>

          </div>
        </section>


        <!-- Persönlichkeit -->
        <section>
          <h2 class="font-serif text-3xl text-stone-900">
            Was mich ausmacht
          </h2>

          <div class="mt-6 space-y-6 text-lg leading-9 text-stone-700">

            <p>
              Mich selbst würde ich als herzlich, empathisch, interessiert,
              naturverbunden, familiär und bodenständig beschreiben.
            </p>

            <p>
              Ich koche gern, bin gerne – vorwiegend wandernd – in der Natur,
              habe eine Katze und liebe es, mich fortzubilden. Man findet mich
              auf Flohmärkten, im Kabarett, Theater oder an irgendeinem See.
            </p>

            <p>
              Familie ist mir sehr wichtig und so findet man mich immer wieder
              in der Steiermark.
            </p>

          </div>
        </section>


        <!-- Beruf -->
        <section class="rounded-3xl bg-stone-900 px-8 py-12 text-stone-100 shadow-xl sm:px-12">

          <span class="text-sm uppercase tracking-[0.3em] text-amber-400">
            Meine Arbeit
          </span>

          <h2 class="mt-4 font-serif text-3xl sm:text-4xl">
            Menschen ganzheitlich sehen
          </h2>

          <div class="mt-8 space-y-6 text-lg leading-9 text-stone-300">

            <p>
              In meine Arbeit als psychologische Beraterin fließen vier Jahrzehnte
              Erfahrung in der Arbeit mit und an Menschen ein.
            </p>

            <p>
              Zahlreiche Ausbildungen helfen mir, Sie ganzheitlich zu erfassen.
              Schon beim Betreten meiner Praxis spricht Ihr Körper mit mir.
            </p>

            <p>
              Je nach Thema, Fragestellung und Auftrag werde ich coachen,
              beraten, supervidieren oder Themen aufstellen.
            </p>

          </div>

        </section>


        <!-- Philosophie -->
        <section class="text-center">

          <div class="mx-auto max-w-3xl">

            <div class="mb-8 text-5xl text-amber-700">
              ❝
            </div>

            <p
              class="font-serif text-2xl leading-relaxed text-stone-700 sm:text-3xl"
            >
              Egal was im Leben passiert, es geht weiter und es lohnt sich
              hinzuschauen und nachzuforschen, um sich seiner bewusst zu werden
              und sich auf die Reise zu sich selbst zu begeben.
            </p>

            <div class="mt-8 text-5xl text-amber-700">
              ❞
            </div>

          </div>

        </section>


        <!-- Abschluss -->
        <section
          class="rounded-3xl bg-linear-to-br from-amber-50 to-stone-100
                 px-8 py-12 text-center ring-1 ring-amber-100 sm:px-16"
        >

          <h2 class="font-serif text-3xl text-stone-900 sm:text-4xl">
            Eine Reise zu sich selbst
          </h2>

          <p class="mx-auto mt-6 max-w-3xl text-lg leading-9 text-stone-600">
            Heute weiß ich: Themen gehören angeschaut. Am besten mit einem
            Gegenüber. Jemandem, der Sie und Ihre Gefühle  ernst nimmt, Ihnen zuhört und mit Ihnen die Ursachen erforscht. 
          </p>

          <p class="mx-auto mt-6 max-w-3xl text-lg leading-9 text-stone-600">
            Vielleicht braucht es Mut, vielleicht einen Ruck oder die
            Überwindung von Angst, um mich zu kontaktieren.
          </p>

          <p class="mt-8 font-serif text-2xl text-amber-800">
            Trauen Sie sich einfach.
          </p>

          <p class="mt-3 text-stone-600">
            Ich bin für Sie da und freue mich darauf, mit Ihnen neue Wege
            zu Ihrem Selbst zu gehen.
          </p>

        </section>


        <!-- Schluss -->
        <footer class="border-t border-stone-200 pt-12 text-center">

          <p
            class="font-serif text-2xl italic text-stone-700 sm:text-3xl"
          >
            „Unsere Reise endet erst mit unserem Tod -
            bis dahin gilt es zu entdecken, zu forschen … zu leben!!!“
          </p>

        </footer>

      </article>

    </main>

  </div>
</template>