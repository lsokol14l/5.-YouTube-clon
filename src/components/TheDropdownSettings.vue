<template>
  <div
    class="sm:right-0 -right-full transition ease-in-out duration-500 absolute bg-white w-72 border border-t-0 top-12 opacity-0 group-hover:opacity-100"
  >
    <!--settings-->
    <section class="py-2 border-b">
      <ul>
        <DropdownSettingsListItem v-for="(item,i) in listItems" :key="i" :label="item.label" :icon="item.icon" :withSubMenu="item.withSubMenu" />
      </ul>
    </section>
    <section class="py-2">
      <ul>
        <li>
          <DropdownSettingsListItem label="Retriced Mod: Off" with-sub-menu/>
        </li>
      </ul>
    </section>
  </div>
</template>

<script setup lang="ts">
import DropdownSettingsListItem from './DropdownSettingsListItem.vue'

const listItems = [
  { label: 'Appearance: Light', icon: 'sun', withSubMenu: true },
  { label: 'Language: English', icon: 'language', withSubMenu: true },
  { label: 'Location: United States', icon: 'location', withSubMenu: true },
  { label: 'Settings', icon: 'settings', withSubMenu: false },
  { label: 'Your data in YouTube', icon: 'data', withSubMenu: false },
  { label: 'Help', icon: 'questionMark', withSubMenu: false },
  { label: 'Send feedback', icon: 'message', withSubMenu: false },
  { label: 'Keyboard shortcuts', icon: 'key', withSubMenu: false }
]
</script>

<style scoped></style>
