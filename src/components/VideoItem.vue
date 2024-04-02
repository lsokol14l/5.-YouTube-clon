<template>
  <a href="/" class="mb-6 group transition">
    <div class="relative text-black">
      <img :src="`https://picsum.photos/seed/image${i}/720/404`" alt="" />
      <span
        class="absolute transition duration-700 bg-opacity-60 opacity-0 group-hover:opacity-100 top-0 right-0 bg-black rounded-sm text-white m-1 p-1"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          viewBox="0 0 20 20"
          fill="currentColor"
        >
          <path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm1-12a1 1 0 10-2 0v4a1 1 0 00.293.707l2.828 2.829a1 1 0 101.415-1.415L11 9.586V6z"
            clip-rule="evenodd"
          />
        </svg>
      </span>
      <span
        class="absolute transition duration-700 bg-opacity-60 opacity-0 group-hover:opacity-100 top-8 right-0 bg-black rounded-sm text-white m-1 p-1"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M4 6h16M4 12h16M4 18h16"
          />
        </svg>
      </span>
      <span
        class="absolute transition duration-700 bottom-0 opacity-100 group-hover:opacity-0 right-0 bg-black rounded-sm text-white m-1 p-1 text-xs font-semibold"
        >6:35</span
      >
    </div>
    <!--description-->
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
          <span>Best Clips</span>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            fill="currentColor"
            class="w-4 h-4 ml-1"
          >
            <path
              fill-rule="evenodd"
              d="M2.25 12c0-5.385 4.365-9.75 9.75-9.75s9.75 4.365 9.75 9.75-4.365 9.75-9.75 9.75S2.25 17.385 2.25 12Zm13.36-1.814a.75.75 0 1 0-1.22-.872l-3.236 4.53L9.53 12.22a.75.75 0 0 0-1.06 1.06l2.25 2.25a.75.75 0 0 0 1.14-.094l3.75-5.25Z"
              clip-rule="evenodd"
            />
          </svg>
        </div>
        <!--views-->
        <div>
          <span> 1M views </span>
          &middot;
          <!--date-->
          <span> 1 year ago </span>
        </div>
      </div>
      <button
        class="ml-auto place-self-start p-1 opacity-0 group-hover:opacity-100 transition duration-700 text-gray-500 hover:text-gray-700 focus:outline-none"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M12 5v.01M12 12v.01M12 19v.01M12 6a1 1 0 110-2 1 1 0 010 2zm0 7a1 1 0 110-2 1 1 0 010 2zm0 7a1 1 0 110-2 1 1 0 010 2z"
          />
        </svg>
      </button>
    </div>
  </a>
</template>

<script setup lang="ts">
defineProps({
  i: Number
})
</script>

<style scoped></style>
