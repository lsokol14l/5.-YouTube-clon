<template>
  <li>
    <a href="/" class="flex items-center px-3 py-1.5 text-sm hover:bg-gray-100">
      <BaseIcon
        name="play"
        class="text-[#ff0000] w-6 h-6 fill-[#ff0000] mr-3"
      />
      <span>{{ title }}</span>
    </a>
  </li>
</template>

<script setup lang="ts">
import BaseIcon from './BaseIcon.vue'

defineProps({
  title: String
})
</script>

<style scoped></style>
