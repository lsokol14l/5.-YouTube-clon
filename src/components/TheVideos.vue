<template>
  <main class="md:ml-24 xl:ml-64 pt-32 px-5 pb-5">
    <div
      class="grid sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 2xl:grid-cols-5 gap-4 max-w-screen-2xl m-auto"
    >
      <VideoItem  v-for="(_item, i) in 20" :key="i" :i="i"/>
    </div>
  </main>
</template>

<script setup lang="ts">
import VideoItem from './VideoItem.vue'
</script>

<style scoped></style>
