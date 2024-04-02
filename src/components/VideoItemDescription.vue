<template>
  <div class="flex items-center mt-3">
    <img
      :src="`https://picsum.photos/seed/avatar${i}/68`"
      class="mr-3 rounded-full w-9 h-9"
      alt=""
    />
    <div class="text-sm">
      <span class="font-semibold text-gray-800">Iron Man vs Spider Man</span>
      <!--channel name-->
      <div class="mt-1 flex items-center">
        <span>Best Clips {{ i }}</span>
        <BaseIcon name="checkCircle" class="w-3.5 h-3.5 ml-1" />
      </div>

      <div>
        <!--views-->
        {{ Number(i) + 1 }}k views &middot;
        <!--date-->
        {{ Number(i) + 1 }} {{ date }} ago
      </div>
    </div>
    <button
      class="ml-auto place-self-start p-1 opacity-0 group-hover:opacity-100 transition duration-700 text-gray-500 hover:text-gray-700 focus:outline-none"
    >
      <BaseIcon name="dotsVertical" />
    </button>
  </div>
</template>

<script setup lang="ts">
import BaseIcon from './BaseIcon.vue'

const props = defineProps({
  i: Number
})
const date = props.i === 0 ? 'day' : 'days'
</script>

<style scoped></style>
