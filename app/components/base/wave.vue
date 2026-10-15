<template>
  <svg 
    class="-my-1 w-full h-auto" 
    :viewBox="`0 0 ${viewBoxWidth} ${viewBoxHeight}`" 
    preserveAspectRatio="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <!-- Top fill: above the sine wave line -->
    <path 
      v-if="topColor" 
      :d="topPath" 
      :fill="topColor"
    />
    
    <!-- Bottom fill: below the sine wave line -->
    <path 
      v-if="bottomColor" 
      :d="bottomPath" 
      :fill="bottomColor"
    />
  </svg>
</template>

<script lang="ts" setup>
interface Props {
  topColor?: string
  bottomColor?: string
  strength?: number
  frequency?: number
  height?: number
}

const props = withDefaults(defineProps<Props>(), {
  strength: 5,
  frequency: 50,
  height: 60
})

const viewBoxWidth = 400
const viewBoxHeight = props.height
const amplitude = props.strength

const centerY = viewBoxHeight / 2

// Generate sample points along the sine wave
function getSinePoints(width: number, freq: number, amp: number): Array<{x: number, y: number}> {
  const points: Array<{x: number, y: number}> = []
  
  for (let x = 0; x <= width; x += 2) {
    const y = amp * Math.sin((x / freq) * 2 * Math.PI) + centerY
    points.push({ x, y })
  }
  
  return points
}

// Top path: rectangle top minus the wave cutout
const topPath = computed(() => {
  const points = getSinePoints(viewBoxWidth, props.frequency, amplitude)
  
  // Start top-left, go to top-right, follow wave backwards, close
  const path: string[] = [
    `M 0 0`,                           // Top-left
    `L ${viewBoxWidth} 0`,             // Top-right
  ]
  
  // Trace wave from right to left
  for (let i = points.length - 1; i >= 0; i--) {
    path.push(`L ${points[i]!.x} ${points[i]!.y}`)
  }
  
  path.push('Z') // Close back to origin
  return path.join(' ')
})

// Bottom path: follow wave forwards, then fill bottom rectangle
const bottomPath = computed(() => {
  const points = getSinePoints(viewBoxWidth, props.frequency, amplitude)
  
  const path: string[] = [
    `M 0 ${centerY}`,                  // Start at center-left
  ]
  
  // Follow wave from left to right
  for (const point of points) {
    path.push(`L ${point.x} ${point.y}`)
  }
  
  path.push(
    `L ${viewBoxWidth} ${viewBoxHeight}`, // Bottom-right
    `L 0 ${viewBoxHeight}`,               // Bottom-left
    'Z'                                   // Close
  )
  
  return path.join(' ')
})
</script>