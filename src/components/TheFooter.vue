<template>
  <div>
    <a v-for="(item, _i) in links.slice(0, 7)" href="/" class="mr-2">{{
      item
    }}</a>
  </div>
  <div>
    <a v-for="(item, _i) in links.slice(7)" href="/" class="mr-2">{{ item }}</a>
  </div>
  <div class="font-normal text-gray-500">&copy; 2024 Google LLC</div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const links = ref([
  'About',
  'Press',
  'Copyright',
  'Contact us',
  'Creators',
  'Advertise',
  'Developers',
  'Terms',
  'Privacy',
  'Policy & Safety',
  'How YouTube works',
  'Test new features'
])
</script>

<style scoped></style>
