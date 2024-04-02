<template>
  <li>
    <a href="/" :class="classes">
      <BaseIcon :class="iconClasses" :name="icon"/>
      <span>{{ label }}</span>
    </a>
  </li>
</template>

<script setup lang="ts">
import BaseIcon from './BaseIcon.vue'
import { computed } from 'vue'

const props = defineProps({
  isActive: Boolean,
  label: String,
  icon: String,
})

const classes = computed(() => {
  const baseClasses = [
    'flex',
    'items-center',
    'py-2',
    'px-6',
    'text-sm',
    'transition-colors',
    'duration-200'
  ]
  return [
    props.isActive
      ? [
          ...baseClasses,
          'font-medium',
          'bg-gray-200',
          'hover:bg-gray-300',
          'text-black'
        ]
      : [...baseClasses, 'hover:bg-gray-100']
  ]
})

const iconClasses = computed(() => {
  const baseClasses = ['w-6', 'h-6', 'mr-6']
  return [...baseClasses, props.isActive ? 'text-[#ff0000]' : '']
})
</script>

<style scoped></style>
