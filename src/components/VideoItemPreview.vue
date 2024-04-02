<template>
  <div class="relative text-black">
    <img :src="`https://picsum.photos/seed/image${i}/720/404`" alt="" />
    <span
      class="absolute transition duration-700 bg-opacity-60 opacity-0 group-hover:opacity-100 top-0 right-0 bg-black rounded-sm text-white m-1 p-1"
    >
      <BaseIcon name="clock" class="h-5 w-5"/>
    </span>
    <span
      class="absolute transition duration-700 bg-opacity-60 opacity-0 group-hover:opacity-100 top-8 right-0 bg-black rounded-sm text-white m-1 p-1"
    >
      <BaseIcon name="videoMenu" class="h-5 w-5"/>  
    </span>
    <span
      class="absolute transition duration-700 bottom-0 opacity-100 group-hover:opacity-0 right-0 bg-black rounded-sm text-white m-1 p-1 text-xs font-semibold"
      >6:35</span
    >
  </div>
</template>

<script setup lang="ts">
import BaseIcon from './BaseIcon.vue'

defineProps({
  i: Number
})
</script>

<style scoped></style>
