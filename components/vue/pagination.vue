<template>
    <div class="items-center p-4 my-4 mx-4 bg-white rounded-2xl shadow-xl shadow-gray-200 sm:flex sm:justify-between">
        <div class="flex items-center mb-4 sm:mb-0">
          <a href="#"
            class="inline-flex justify-center p-1 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
            
            <ChevronLeftIcon  class="w-7 h-7"/>
          </a>
          <a href="#"
            class="inline-flex justify-center p-1 mr-2 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
            <ChevronRightIcon  class="w-7 h-7"/>
          </a>
          <span class="text-sm font-normal text-gray-500">Showing <span class="font-semibold text-gray-900">1-20</span>
            of <span class="font-semibold text-gray-900">2290</span></span>
        </div>
        <div class="flex items-center space-x-3">
          <a href="#"
            class="inline-flex flex-1 justify-center items-center py-2 px-3 text-sm font-medium text-center text-white bg-gradient-to-br from-dark-700 to-dark-900 rounded-lg shadow-md shadow-gray-300 hover:scale-[1.02] transition-transform">
            
            <ChevronLeftIcon  class="mr-1 -ml-1 w-5 h-5"/>
            Previous
          </a>
          <a href="#"
            class="inline-flex flex-1 justify-center items-center py-2 px-3 text-sm font-medium text-center text-white bg-gradient-to-br from-dark-700 to-dark-900 rounded-lg shadow-md shadow-gray-300 hover:scale-[1.02] transition-transform">
            Next
            
            <ChevronRightIcon  class="ml-1 -mr-1 w-5 h-5"/>
          </a>
        </div>
      </div>
</template>
<script setup>
import { ChevronLeftIcon, ChevronRightIcon } from '@heroicons/vue/solid';

</script>