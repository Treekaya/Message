<template>
  <nav class="w-full bg-white relative z-50">
    <!-- Desktop Navigation -->
    <div class="hidden lg:block">
      <div class="max-w-6xl mx-auto px-4">
        <div class="flex justify-center items-center gap-6 py-4">
          <a href="/" 
             class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-blue-50 hover:text-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-400">
            Home
          </a>
          
          <a href="/angebot" 
             class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-green-50 hover:text-green-700 focus:outline-none focus:ring-2 focus:ring-green-400">
            Angebot
          </a>
          
          <a href="/massage" 
             class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-purple-50 hover:text-purple-700 focus:outline-none focus:ring-2 focus:ring-purple-400">
            Massage
          </a>
          
          <a href="/ueber-mich" 
             class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-teal-50 hover:text-teal-700 focus:outline-none focus:ring-2 focus:ring-teal-400">
            Über mich
          </a>

          <a href="/kontakt" 
             class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-orange-50 hover:text-orange-700 focus:outline-none focus:ring-2 focus:ring-orange-400">
            Kontakt
          </a>
        </div>
      </div>
    </div>

    <!-- Mobile -->
    <div class="lg:hidden">
      <div class="max-w-6xl mx-auto px-4 py-4 flex justify-between items-center">
        
        <span class="font-semibold text-gray-800">Massagepraxis Köck</span>
        
        <button 
          @click="toggleMenu" 
          class="focus:outline-none focus:ring-2 focus:ring-blue-400 rounded-lg p-2"
          aria-label="Menü öffnen"
        >
          <svg 
            v-if="!menuOpen" 
            xmlns="http://www.w3.org/2000/svg" 
            class="h-6 w-6 text-gray-700" 
            fill="none" 
            viewBox="0 0 24 24" 
            stroke="currentColor"
          >
            <path 
              stroke-linecap="round" 
              stroke-linejoin="round" 
              stroke-width="2" 
              d="M4 6h16M4 12h16M4 18h16" 
            />
          </svg>
          <svg 
            v-else 
            xmlns="http://www.w3.org/2000/svg" 
            class="h-6 w-6 text-gray-700" 
            fill="none" 
            viewBox="0 0 24 24" 
            stroke="currentColor"
          >
            <path 
              stroke-linecap="round" 
              stroke-linejoin="round" 
              stroke-width="2" 
              d="M6 18L18 6M6 6l12 12" 
            />
          </svg>
        </button>
      </div>

      <!-- Dropdown -->
      <transition
        enter-active-class="transition duration-200 ease-out"
        enter-from-class="opacity-0 -translate-y-2"
        enter-to-class="opacity-100 translate-y-0"
        leave-active-class="transition duration-150 ease-in"
        leave-from-class="opacity-100 translate-y-0"
        leave-to-class="opacity-0 -translate-y-2"
      >
        <div 
          v-if="menuOpen" 
          class="absolute top-full left-0 right-0 bg-white border-t border-gray-100 shadow-lg py-4 px-4 flex flex-col gap-3"
        >
          <a 
            href="/" 
            class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-blue-50 hover:text-blue-700 text-center"
            @click="closeMenu"
          >
            Home
          </a>
          
          <a 
            href="/angebot" 
            class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-green-50 hover:text-green-700 text-center"
            @click="closeMenu"
          >
            Angebot
          </a>
          
          <a 
            href="/massage" 
            class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-purple-50 hover:text-purple-700 text-center"
            @click="closeMenu"
          >
            Massage
          </a>
          
          <a 
            href="/ueber-mich" 
            class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-teal-50 hover:text-teal-700 text-center"
            @click="closeMenu"
          >
            Über mich
          </a>

          <a 
            href="/kontakt" 
            class="px-6 py-3 rounded-lg font-medium text-gray-700 transition-all hover:bg-orange-50 hover:text-orange-700 text-center"
            @click="closeMenu"
          >
            Kontakt
          </a>
        </div>
      </transition>
    </div>
  </nav>
  
  <BaseWave top-color="#fff" :height="10" :frequency="800" class="relative z-40" />
</template>

<script setup>
import { ref } from 'vue'

const menuOpen = ref(false)

const toggleMenu = () => {
  menuOpen.value = !menuOpen.value
}

const closeMenu = () => {
  menuOpen.value = false
}

onMounted(() => {
  const handleEsc = (event) => {
    if (event.key === 'Escape') {
      closeMenu()
    }
  }
  
  window.addEventListener('keydown', handleEsc)
  onUnmounted(() => {
    window.removeEventListener('keydown', handleEsc)
  })
})
</script>