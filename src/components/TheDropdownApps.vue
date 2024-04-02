<template>
  <div
    class="right-0 sm:left-0 transition ease-in-out duration-500 absolute bg-white w-60 border border-t-0 top-12 opacity-0 group-hover:opacity-100"
  >
    <!--first apps section-->
    <section class="py-2 border-b">
      <ul>
        <DropdownAppsListItem title="YouTube TV" />
      </ul>
    </section>
    <!--second apps section-->
    <section class="py-2 border-b">
      <ul>
        <DropdownAppsListItem title="YouTube Music" />
        <DropdownAppsListItem title="YouTube Kids" />
      </ul>
    </section>
    <!--third apps section-->
    <section class="py-2">
      <ul>
        <DropdownAppsListItem title="Creator Academy" />
        <DropdownAppsListItem title="YouTube for Artist" />
      </ul>
    </section>
  </div>
</template>

<script setup lang="ts">
import DropdownAppsListItem from './DropdownAppsListItem.vue'
</script>

<style scoped></style>
