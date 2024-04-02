<template>
  <li>
    <a href="/" class="flex items-center px-4 py-2 text-sm hover:bg-gray-100">
      <BaseIcon v-if="icon" :name="icon" class="w-7 h-7 text-gray-400 mr-3 pt-1" />
      <span>{{ label }}</span>
      <BaseIcon
        name="theNextArrow"
        v-if="withSubMenu"
        class="w-5 h-5 text-gray-400 ml-auto"
      />
    </a>
  </li>
</template>

<script setup lang="ts">
import BaseIcon from './BaseIcon.vue'

defineProps({
  icon: String,
  label: String,
  withSubMenu: Boolean
})
</script>

<style scoped></style>
