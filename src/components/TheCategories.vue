<template>
  <section
    class="md:pl-24 xl:pl-64 w-full pt-14 fixed z-10 opacity-95 bg-white"
  >
    <div class="border-t border-b px-4 max-w-screen-2xl m-auto">
      <div
        class="py-3 flex space-x-3 overflow-auto no-scrollbar text-sm whitespace-nowrap"
      >
        <CategoryItem
          v-for="(category, _i) in categories"
          :key="category"
          :category="category"
          :is-active="category==='All'"
        />
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import CategoryItem from './CategoryItem.vue'

const categories = ref([
  'All',
  'Trucks',
  'Tools',
  'Machines',
  'Engines',
  'Show',
  'Ships',
  'Roads',
  'Tanks',
  'Building',
  'Mars',
  'Woodworking',
  'Tracktors',
  'Songs',
  'Tv Shows',
  'Football',
  'Planes',
  'Live',
  'Streeets',
  'Math',
  'Programming'
])
</script>

<style scoped></style>
