<template>
  <header class="flex justify-between fixed z-30 w-full">
    <!--left header bar-->
    <div class="lg:w-1/4 flex">
      <div class="flex items-center xl:w-64 xl:bg-white pl-4">
        <!--burger menu-->
        <button class="mr-3 sm:ml-2 sm:mr-6 focus:outline-none">
          <BaseIcon name="menu" />
        </button>
        <!--YouTube logo-->
        <LogoMain />
      </div>
    </div>
    <!--mid header bar (search)-->
    <div
      class="hidden lg:w-1/2 sm:flex flex-1 justify-end pl-8 md:pl-12 md:px-8 lg:px-0 items-center p-2.5 max-w-screen-md"
    >
      <div class="flex w-full h-full">
        <TheSearch />
      </div>
      <button class="ml-4 focus:outline-none">
        <BaseIcon name="microphone" class="w-5 h-5" />
      </button>
    </div>
    <!--right header bar-->
    <div
      class="lg:w-1/4 flex items-center justify-end sm:space-x-3 p-2 sm:px-4"
    >
      <button class="sm:hidden p-2 focus:outline-none">
        <BaseIcon name="microphone" class="w-5 h-5" />
      </button>
      <button class="sm:hidden p-2 focus:outline-none">
        <BaseIcon name="search" class="w-5 h-5" />
      </button>
      <!--button more apps-->
      <button class="relative group p-2 focus:outline-none">
        <BaseIcon name="viewGrid" class="w-5 h-5" />
        <TheDropdownApps />
      </button>
      <!--settings button-->
      <button class="relative group p-2 focus:outline-none">
        <BaseIcon name="dotsVertical" class="w-5 h-5" />
        <TheDropdownSettings />
      </button>
      <ButtonLogin />
    </div>
  </header>
</template>

<script setup lang="ts">
import TheDropdownApps from './TheDropdownApps.vue'
import TheDropdownSettings from './TheDropdownSettings.vue'
import LogoMain from './LogoMain.vue'
import TheSearch from './TheSearch.vue'
import ButtonLogin from './ButtonLogin.vue'
import BaseIcon from './BaseIcon.vue'
</script>

<style scoped></style>
