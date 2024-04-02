<script setup lang="ts">
import { computed } from 'vue'
import '../icons'
import BaseIcon from './BaseIcon.vue'

const props = defineProps({
  class: String
})

const classes = computed(() => {
  return [
    'flex',
    'focus:outline-none',
    'whitespace-nowrap',
    'items-center',
    'px-2',
    'py-1',
    'text-sm',
    'uppercase',
    'text-blue-600',
    'border',
    'border-blue-600',
    'rounded-sm',
    'hover:bg-blue-600',
    'hover:text-white',
    props.class
  ]
})
</script>

<template>
  <button :class="classes">
    <BaseIcon name="userCircle" class="mr-2 h-7 w-7 fill-[#2563eb] text-white" />
    Sign In
  </button>
</template>
