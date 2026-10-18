<template>
  <div class="flex gap-5">
              <div class="mt-2 h-3 w-3 shrink-0 rounded-full bg-amber-700 ring-4 ring-amber-100"></div>

              <div>
                <span class="text-sm font-semibold uppercase tracking-widest text-amber-700">
                  {{ title }}
                </span>
                <p class="mt-2 leading-8 text-stone-600">
                  {{ text }}
                </p>
              </div>
            </div>
</template>

<script lang="ts" setup>
defineProps<{
  title: string
  text: string
}>()
</script>