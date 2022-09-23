<template>
    <div
        class="FooterNav p-2 bg-slate-900 fixed top-auto bottom-0 inset-x-0 z-30 border-t border-neutral-300 dark:border-neutral-700  transition-transform duration-300 ease-in-out">
        <div class="w-full max-w-lg flex justify-around mx-auto text-sm text-center ">
            <NuxtLink class="flex flex-col items-center justify-between text-neutral-500 dark:text-neutral-300/90 "
                to="/">
                <HomeIcon class="w-6 h-6 " />
                <span class="text-[11px] leading-none mt-1">Home</span>
            </NuxtLink>
            <NuxtLink class="flex flex-col items-center justify-between text-neutral-500 dark:text-neutral-300/90 "
                to="/about">
                <IdentificationIcon class="w-6 h-6 " />
                <span class="text-[11px] leading-none mt-1">Wishlists</span>
            </NuxtLink>
            <NuxtLink class="flex flex-col items-center justify-between text-neutral-500 dark:text-neutral-300/90 "
                to="/rooms">
                <OfficeBuildingIcon class="w-6 h-6" />
                <span class="text-[11px] leading-none mt-1">Rooms</span>
            </NuxtLink>
            <NuxtLink class="flex flex-col items-center justify-between text-neutral-500 dark:text-neutral-300/90 "
                to="/rooms">
                <PhotographIcon class="w-6 h-6" />
                <span class="text-[11px] leading-none mt-1">Gallery</span>
            </NuxtLink>
            <NuxtLink class="flex flex-col items-center justify-between text-neutral-500 dark:text-neutral-300/90 "
                to="/rooms">
                <PhoneIcon class="w-6 h-6" />
                <span class="text-[11px] leading-none mt-1">Contact</span>
            </NuxtLink>
        </div>
    </div>
</template>

<script setup>
import { HomeIcon, MenuIcon, PhoneIcon, OfficeBuildingIcon, PhotographIcon, IdentificationIcon } from '@heroicons/vue/solid';

</script >