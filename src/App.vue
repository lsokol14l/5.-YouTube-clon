<script setup lang="ts">
import TheHeader from './components/TheHeader.vue'
import SmallSidebar from './components/SmallSidebar.vue'
import TheSidebar from './components/TheSidebar.vue'
import TheCategories from './components/TheCategories.vue'
import MobileSidebar from './components/MobileSidebar.vue'
import Videos from './components/TheVideos.vue'
</script>

<template>
  <body class="text-gray-600 bg-gray-50">
    <!--header-->
    <TheHeader />
    
    <!--small sidebar-->
    <SmallSidebar />

    <!--sidebar menu-->
    <TheSidebar />

    <!--mobile sidebar wrapper-->
    <MobileSidebar />

    <!--categories(trash realisation don't open)-->
    <TheCategories />

    <!--videos-->
    <Videos />
  </body>
</template>

<style scoped></style>
