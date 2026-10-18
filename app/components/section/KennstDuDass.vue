
<template>
  <section class="relative overflow-hidden bg-[#e8ddcd]">

    <div class="relative z-10">
      <BaseWave
        top-color="#faf8f4"
        bottom-color="#e8ddcd"
        :strength="3"
        :frequency="200"
      />
    </div>

    <!-- Dekorativer Kreis oben rechts -->
    <div
      class="pointer-events-none absolute -right-64 top-42
             h-96 w-96 rounded-full bg-[#6d4aff]/8"
    ></div>

    <!-- Dekorativer Kreis unten links -->
    <div
      class="pointer-events-none absolute -bottom-40 -left-32
             h-96 w-96 rounded-full bg-white/30"
    ></div>

    <!-- Inhalt -->
    <BaseContent class="relative z-10 py-24 sm:py-32">

      <div class="mx-auto max-w-4xl text-center">

        <span
          class="inline-flex items-center gap-3
                 text-sm font-semibold uppercase tracking-[0.25em]
                 text-[#806b53]"
        >
          <span class="h-px w-8 bg-[#806b53]"></span>
          Kennen Sie das …
          <span class="h-px w-8 bg-[#806b53]"></span>
        </span>

        <h2
          class="mt-10 min-h-28 font-serif text-3xl
                 leading-relaxed text-blue-950
                 sm:min-h-32 sm:text-5xl"
          aria-live="polite"
          aria-atomic="true"
        >
          {{ displayedText }}<span
            class="ml-1 inline-block h-7 w-px
                   translate-y-1 animate-pulse bg-[#6d4aff]
                   sm:h-10"
            aria-hidden="true"
          ></span>
        </h2>

        <!-- Dezenter Abschluss -->
        <div
          class="mx-auto mt-10 h-px w-16 bg-[#806b53]/50"
        ></div>

      </div>

    </BaseContent>

  </section>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const texts = [
  'Ich fühle mich so einsam.',
  'Ich bin so traurig.',
  'Ich habe ständig Angst.',
  'Ich fühle mich so überfordert.',
  'Ich funktioniere nur mehr.',
  'In meiner Beziehung stimmt überhaupt nichts mehr.',
  'Niemand hört mir zu.',
  'Ich bin so schüchtern.',
  'Ich weiß nicht mehr weiter.'
]

const displayedText = ref('')

let timer
let currentIndex = -1
let charIndex = 0
let deleting = false

function nextIndex() {
  if (texts.length <= 1) return 0

  let index

  do {
    index = Math.floor(Math.random() * texts.length)
  } while (index === currentIndex)

  return index
}

function animateText() {
  const text = texts[currentIndex]

  if (!deleting) {
    charIndex++
    displayedText.value = text.slice(0, charIndex)

    if (charIndex >= text.length) {
      deleting = true
      timer = setTimeout(animateText, 2200)
      return
    }

    timer = setTimeout(animateText, 65)
  } else {
    charIndex--
    displayedText.value = text.slice(0, charIndex)

    if (charIndex <= 0) {
      deleting = false
      currentIndex = nextIndex()
      timer = setTimeout(animateText, 400)
      return
    }

    timer = setTimeout(animateText, 30)
  }
}

onMounted(() => {
  currentIndex = nextIndex()
  animateText()
})

onUnmounted(() => {
  clearTimeout(timer)
})
</script>