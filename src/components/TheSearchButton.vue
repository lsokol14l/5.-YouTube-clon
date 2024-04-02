<script setup lang="ts">
import BaseIcon from './BaseIcon.vue'
</script>

<template>
  <button
    class="border focus:outline-none border-l-transparent hover:bg-gray-200 rounded-r-sm flex items-center px-6 py-1 text-gray-600 bg-gray-100"
  >
    <svg
      xmlns="http://www.w3.org/2000/svg"
      fill="none"
      viewBox="0 0 24 24"
      stroke-width="1.5"
      stroke="currentColor"
      class="w-5 h-5"
    >
      <BaseIcon name="search" class="w-5 h-5"/>
    </svg>
  </button>
</template>
