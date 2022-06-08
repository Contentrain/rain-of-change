<template>
  <span
    :class="tailwindColors[tag.color]"
    class="px-2 py-1 mr-2 rounded-lg text-sm"
  >{{ tag.text }}
  </span>
</template>

<script setup>
// eslint-disable-next-line @typescript-eslint/no-unused-vars
const props = defineProps({
  tag: {
    type: Object,
    required: true
  }
})
const tailwindColors = {
  blue: 'bg-blue-100 text-blue-500',
  red: 'bg-red-100 text-red-500',
  yellow: 'bg-yellow-100 text-yellow-500',
  gray: 'bg-gray-100 text-gray-500',
  zinc: 'bg-zinc-100 text-zinc-500',
  green: 'bg-green-100 text-green-500',
  purple: 'bg-purple-100 text-purple-500',
  orange: 'bg-orange-100 text-orange-500',
  pink: 'bg-pink-100 text-pink-500',
  teal: 'bg-teal-100 text-teal-500',
  indigo: 'bg-indigo-100 text-indigo-500',
  cyan: 'bg-cyan-100 text-cyan-500',
  brown: 'bg-brown-100 text-brown-500',
  slate: 'bg-slate-100 text-slate-500',
  amber: 'bg-amber-100 text-amber-500',
  lime: 'bg-lime-100 text-lime-500',
  emerald: 'bg-emerald-100 text-emerald-500',
  sky: 'bg-sky-100 text-sky-500'
}

</script>
