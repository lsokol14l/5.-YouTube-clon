<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    fill="none"
    viewBox="0 0 24 24"
    stroke-width="1.5"
    stroke="currentColor"
    :class="$attrs.class || 'w-6 h-6'"
    v-html="path"
  ></svg>
</template>

<script setup lang="ts">
import icons from '../icons'
const props = defineProps({
  name: String
})

const path = icons[props.name as keyof typeof icons]
</script>
