<script setup lang="ts">
import '../icons'
import BaseIcon from './BaseIcon.vue'
</script>

<template>
  <button
    class="flex focus:outline-none whitespace-nowrap items-center px-2 py-1 text-sm uppercase text-blue-600 border border-blue-600 rounded-sm"
  >
    <BaseIcon name="user" class="mr-2 h-7 w-7 fill-white text-[#2563eb]" />
    Sign In
  </button>
</template>
