<template>
  <a href="" :class="classes">{{ category }}</a>
</template>

<script lang="ts" setup>
import { defineProps, ref } from 'vue'
const props = defineProps({
  category: String,
  isActive: Boolean
})

const classes = ref([
  'px-3',
  'py-1',
  'transition',
  'border',
  'border-gray-300',
  'rounded-full',
  'bg-gray-200',
  'hover:bg-gray-300'
])
// 'border-gray-700', 'hover:bg-gray-500', 'text-white', 'bg-gray-600'
if (props.isActive) {
  classes.value.push(
    'border-gray-700',
    'hover:bg-gray-500',
    'text-white',
    'bg-gray-600'
  )
}
</script>

<style scoped></style>
