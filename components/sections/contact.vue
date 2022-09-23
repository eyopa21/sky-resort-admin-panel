<template>
    <div class="nc-SectionSubscribe2 relative flex flex-col lg:flex-row lg:items-center "
        data-nc-id="SectionSubscribe2">
        <div class="flex-shrink-0 mb-10 lg:mb-0 lg:mr-10 lg:w-2/5">
            <h2 class="font-semibold text-4xl">Contact us 🎉</h2><span
                class="block mt-5 text-neutral-500 dark:text-neutral-400">Ask anything or leave us any appreciation comment here...</span>
            <ul class="space-y-4 mt-10">
                <li class="flex items-center space-x-4"><span
                        class="nc-Badge inline-flex px-2.5 py-1 rounded-full font-medium text-xs relative text-blue-800 bg-blue-100  relative">01</span><span
                        class="font-medium text-neutral-700 dark:text-neutral-300">Get more
                        discount</span></li>
                <li class="flex items-center space-x-4"><span
                        class="nc-Badge inline-flex px-2.5 py-1 rounded-full font-medium text-xs relative text-red-800 bg-red-100  relative">02</span><span
                        class="font-medium text-neutral-700 dark:text-neutral-300">Get premium
                        magazines</span></li>
            </ul>
            <form class="mt-10 relative max-w-sm"><input type="email"
                    class="block w-full border-neutral-200 focus:border-primary-300 focus:ring focus:ring-primary-200 focus:ring-opacity-50 bg-white dark:border-neutral-700 dark:focus:ring-primary-6000 dark:focus:ring-opacity-25 dark:bg-neutral-900 rounded-full text-sm font-normal h-11 px-4 py-3 "
                    required aria-required="true" placeholder="Enter your email"><button
                    class="ttnc-ButtonCircle flex items-center justify-center rounded-full !leading-none disabled:bg-opacity-70 bg-primary-6000 hover:bg-primary-700 text-neutral-50 absolute transform top-1/2 -translate-y-1/2 right-[5px]  w-9 h-9  focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-primary-6000 dark:focus:ring-offset-0"
                    type="submit"><ArrowRightIcon class="w-5 h-5"/></button></form>
        </div>
        <div class="flex-grow">
            <div class="nc-NcImage " data-nc-id="NcImage">
                <div
                    class="object-cover w-full h-full flex items-center justify-center bg-neutral-200 dark:bg-neutral-6000 text-neutral-100 dark:text-neutral-500">
                    <div class="w-full h-full">
                        <img class="w-full h-full" src="../../assets/img/unity.jpg" alt="">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ArrowRightIcon } from '@heroicons/vue/solid';

</script>