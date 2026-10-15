<template>
  <article
    class="group overflow-hidden rounded-3xl bg-white shadow-sm
            ring-1 ring-stone-200 transition duration-300
            hover:-translate-y-1 hover:shadow-xl"
  >

    <div class="grid md:grid-cols-[220px_1fr]">

      <!-- linke Seite -->
      <div
        class="relative flex min-h-55 flex-col justify-between
                overflow-hidden bg-[#6d4aff] p-8 text-white"
      >

        <!-- dekorativer Kreis -->
        <div
          class="absolute -right-16 -top-16 h-40 w-40 rounded-full
                  bg-white/10"
        ></div>

        <div
          class="absolute -bottom-20 -left-10 h-48 w-48 rounded-full
                  bg-black/10"
        ></div>

        <div class="relative mt-auto">
          <div class="mb-4 text-5xl">
            ♡
          </div>

          <h2 class="font-serif text-2xl">
            Beziehungen
          </h2>
        </div>

      </div>


      <!-- Inhalt -->
      <div class="p-8 md:p-10">

        <h3 class="font-serif text-2xl text-stone-900">
          Beziehungen klären
        </h3>

        <p class="mt-4 text-lg font-medium leading-8 text-[#6d4aff]">
          Unstimmigkeiten mit dem Partner, dem Kollegen,
          in Freundschaften oder in der Familie?
        </p>

        <p class="mt-5 leading-8 text-stone-600">
          Da man den anderen nicht ändern kann, ist es wichtig,
          seine eigenen Bedürfnisse zu erkennen und diese klar zu
          kommunizieren.
        </p>

        <p class="mt-4 leading-8 text-stone-600">
          Entweder gelingt es Ihnen dadurch, sich Ihrem Gegenüber
          wieder anzunähern, oder es läuft auf einen respektvollen
          Abschied – sofern das möglich ist – hinaus.
        </p>

      </div>

    </div>
  </article>
</template>