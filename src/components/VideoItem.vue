<template>
  <a href="/" class="mb-6 group transition">
    <VideoItemPreview :i="i"/>
    <!--description-->
    <VideoItemDescription :i="i" />
  </a>
</template>

<script setup lang="ts">
import VideoItemPreview from './VideoItemPreview.vue'
import VideoItemDescription from './VideoItemDescription.vue'


defineProps({
  i: Number
})
</script>

<style scoped></style>
