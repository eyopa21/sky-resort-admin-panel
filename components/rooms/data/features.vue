<template>
    <div class="listingSection__wrap">
        <div>
            <h2 class="text-2xl font-semibold">Amenities </h2><span
                class="block mt-2 text-neutral-500 dark:text-neutral-400">About the
                property's amenities and services</span>
        </div>
        <div class="w-14 border-b border-neutral-200 dark:border-neutral-700"></div>
        <div
            class="grid grid-cols-1 xl:grid-cols-3 gap-6 text-sm text-neutral-700 dark:text-neutral-300 ">
            <div v-for="i in 8" :key="i" class="flex items-center space-x-3"><KeyIcon class="w-5 h-5"/><span class=" ">Electronic key</span></div>
           
            
        </div>
        <div class="w-14 border-b border-neutral-200"></div>
        <div><button
                class="nc-Button relative h-auto inline-flex items-center justify-center rounded-full transition-colors text-sm sm:text-base px-4 py-3 sm:px-6  ttnc-ButtonSecondary font-medium border bg-white border-neutral-200 text-neutral-700 dark:bg-neutral-900 dark:text-neutral-300 dark:border-neutral-700 hover:bg-neutral-100 dark:hover:bg-neutral-800   focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-primary-6000 dark:focus:ring-offset-0">
                Contact us</button></div>
    </div>
</template>
<script setup>
import { KeyIcon } from '@heroicons/vue/solid';

</script>