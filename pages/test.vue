<template>
  <div class="bg-white">
    <div
    class="block justify-between items-center p-4 mx-4 mt-4 mb-6 bg-white rounded-2xl shadow-xl shadow-gray-200 lg:p-5 sm:flex">
    <div class="mb-1 w-full">
      <div class="mb-4">

        <h1 class="text-xl font-semibold text-gray-900 sm:text-2xl">All Rooms</h1>
      </div>
      <div class="sm:flex">
        <div class="hidden items-center mb-3 sm:flex sm:divide-x sm:divide-gray-100 sm:mb-0">
          <form class="lg:pr-3">
            <label for="users-search" class="sr-only">Search</label>
            <div class="relative mt-1 lg:w-64 xl:w-96">
              <input type="text" name="email" id="users-search"
                class="border border-gray-300 text-gray-900 sm:text-sm rounded-lg focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300 block w-full p-2.5"
                placeholder="Search for users">

            </div>
          </form>
          <div class="flex pl-0 mt-3 space-x-1 sm:pl-2 sm:mt-0">
            <a href="#"
              class="inline-flex justify-center p-1 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">

              <CogIcon class="w-6 h-6" />
            </a>
            <a href="#"
              class="inline-flex justify-center p-1 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
              <CogIcon class="w-6 h-6" />
            </a>
            <a href="#"
              class="inline-flex justify-center p-1 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
              <CogIcon class="w-6 h-6" />
            </a>
            <a href="#"
              class="inline-flex justify-center p-1 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
              <CogIcon class="w-6 h-6" />
            </a>
          </div>
        </div>
        <div class="flex items-center ml-auto space-x-2 sm:space-x-3">
          <button type="button" data-modal-toggle="add-user-modal"
            class="inline-flex items-center py-2 px-3 text-sm font-medium text-center text-white rounded-lg bg-gradient-to-br from-pink-500 to-voilet-500 sm:ml-auto shadow-md shadow-gray-300 hover:scale-[1.02] transition-transform">

            <PlusIcon class="mr-2 -ml-1 w-6 h-6" />
            Add user
          </button>

        </div>
      </div>
    </div>
  </div>
  
  <div class="grid grid-cols-1 md:grid-cols-2 md:gap-6  pl-4 md:p-4">

    <div v-for="i in 9" :key="i" class=" py-8 flex justify-center border-2 w-full" >

      <div v-for="(i, key) in images" :key="key">

        <div v-if="key==slider" class=" bg-gray-50 w-full ">

          <!-- Carousel Body -->
          <div class="w-full h-full relative rounded-lg  bg-gray-100 shadow-xl" style="min-height: 19rem;">
            <div class="relative w-full h-full overflow-hidden rounded-lg" style="min-height: 19rem;">
              <img class="absolute inset-0 w-full h-full object-fit object-center" :src="i" alt="">

              <div class="absolute inset-0 w-full h-full flex items-center justify-center fill-current text-white">

              </div>
            </div>
            <div class="w-full h-full flex items-center bg-gray-100 rounded-lg">
              <div class="p-4 absolute bottom-0 pl-16 flex justify-center">
                <p class="text-gray-600"><span class="text-gray-900">Missguided</span> </p>

              </div>
            </div>
            <button @click="prev()"
              class="absolute top-0 mt-32 left-0 bg-white rounded-full shadow-md h-12 w-12 text-2xl text-indigo-600 hover:text-indigo-400 focus:text-indigo-400 -ml-6 focus:outline-none focus:shadow-outline">
              <span class="block" style="transform: scale(-1);">&#x279c;</span>
            </button>
            <button @click="next()"
              class="absolute top-0 mt-32 right-0 bg-white rounded-full shadow-md h-12 w-12 text-2xl text-indigo-600 hover:text-indigo-400 focus:text-indigo-400 -mr-6 focus:outline-none focus:shadow-outline">
              <span class="block" style="transform: scale(1);">&#x279c;</span>
            </button>
          </div>

          <!-- Carousel Tabs -->
          <div class="flex items-center pt-2 justify-center ">
            <button v-for="i in 5" :key="i" class="px-1 opacity-50 hover:opacity-100 focus:opacity-100"><img class="w-full"
                src="../assets/img/1.png" alt="" style="max-height: 40px;"></button>
            
          </div>

          <!-- Display Container (not part of component) END -->

        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script setup>
   import {
    CogIcon,
    PlusIcon,
    TrashIcon,
    PencilAltIcon
  } from "@heroicons/vue/outline";
  definePageMeta({
    middleware: "navigation-guard"
  })
  import {
    ref
  } from "vue";
  import {
    MenuIcon,
    XIcon
  } from "@heroicons/vue/outline";
  const slider = ref(0);
  const images = ref([
    '../assets/img/1.png',
    '../assets/img/unity.jpg',
    '../assets/img/eyoba.jpg'
  ])
  const next = () => {
    console.log("next", slider.value)
    slider.value++;
    if (slider.value == images.value.length) {
      slider.value = 0;
    }
  }
  const prev = () => {
    console.log("prev")
    slider.value++;
    if (slider.value == images.value.length) {
      slider.value = images.value.length;
    }
  }
</script>