<template>
    <div class="absolute right-0 z-10 w-full sm:min-w-[340px] max-w-sm bg-white dark:bg-neutral-800 top-full mt-3 py-5 sm:py-6 px-4 sm:px-8 rounded-3xl shadow-xl opacity-100 translate-y-0"
        id="headlessui-popover-panel-:r7r:" tabindex="-1">
        <div class="nc-NcInputNumber flex items-center justify-between space-x-5 w-full" data-nc-id="NcInputNumber">
            <div class="flex flex-col"><span
                    class="font-medium text-neutral-800 dark:text-neutral-200">Adults</span><span
                    class="text-xs text-neutral-500 dark:text-neutral-400 font-normal">Ages 13 or above</span></div>
            <div class="nc-NcInputNumber flex items-center justify-between w-28"><button
                @click="subAdult"
                    class="w-8 h-8 rounded-full flex items-center justify-center border border-neutral-400 dark:border-neutral-500 bg-white dark:bg-neutral-900 focus:outline-none hover:border-neutral-700 disabled:hover:border-neutral-400 dark:disabled:hover:border-neutral-500 disabled:opacity-50 disabled:cursor-default"
                    type="button">
                    <MinusIcon class="w-5 h-5" />

                </button><span>{{amount.adult}}</span><button
                @click="addAdult"
                    class="w-8 h-8 rounded-full flex items-center justify-center border border-neutral-400 dark:border-neutral-500 bg-white dark:bg-neutral-900 focus:outline-none hover:border-neutral-700 disabled:hover:border-neutral-400 dark:disabled:hover:border-neutral-500 disabled:opacity-50 disabled:cursor-default"
                    type="button">
                    <PlusIcon class="w-5 h-5" />
                </button></div>
        </div>
        <div class="nc-NcInputNumber flex items-center justify-between space-x-5 w-full mt-6"
            data-nc-id="NcInputNumber">
            <div class="flex flex-col"><span
                    class="font-medium text-neutral-800 dark:text-neutral-200">Children</span><span
                    class="text-xs text-neutral-500 dark:text-neutral-400 font-normal">Ages 2–12</span></div>
            <div class="nc-NcInputNumber flex items-center justify-between w-28"><button
                @click="subChild"
                    class="w-8 h-8 rounded-full flex items-center justify-center border border-neutral-400 dark:border-neutral-500 bg-white dark:bg-neutral-900 focus:outline-none hover:border-neutral-700 disabled:hover:border-neutral-400 dark:disabled:hover:border-neutral-500 disabled:opacity-50 disabled:cursor-default"
                    type="button">
                    <MinusIcon class="w-5 h-5" />
                </button><span>{{amount.children}}</span><button
                @click="addChild"
                    class="w-8 h-8 rounded-full flex items-center justify-center border border-neutral-400 dark:border-neutral-500 bg-white dark:bg-neutral-900 focus:outline-none hover:border-neutral-700 disabled:hover:border-neutral-400 dark:disabled:hover:border-neutral-500 disabled:opacity-50 disabled:cursor-default"
                    type="button">
                    <PlusIcon class="w-5 h-5" />
                </button></div>
        </div>
        <div class="nc-NcInputNumber flex items-center justify-between space-x-5 w-full mt-6"
            data-nc-id="NcInputNumber">
            <div class="flex flex-col"><span
                    class="font-medium text-neutral-800 dark:text-neutral-200">Infants</span><span
                    class="text-xs text-neutral-500 dark:text-neutral-400 font-normal">Ages 0–2</span></div>
            <div class="nc-NcInputNumber flex items-center justify-between w-28"><button
                @click="subInfant"
                    class="w-8 h-8 rounded-full flex items-center justify-center border border-neutral-400 dark:border-neutral-500 bg-white dark:bg-neutral-900 focus:outline-none hover:border-neutral-700 disabled:hover:border-neutral-400 dark:disabled:hover:border-neutral-500 disabled:opacity-50 disabled:cursor-default"
                    type="button">
                    <MinusIcon class="w-5 h-5" />
                </button><span>{{amount.infant}}</span><button
                @click="addInfant"
                    class="w-8 h-8 rounded-full flex items-center justify-center border border-neutral-400 dark:border-neutral-500 bg-white dark:bg-neutral-900 focus:outline-none hover:border-neutral-700 disabled:hover:border-neutral-400 dark:disabled:hover:border-neutral-500 disabled:opacity-50 disabled:cursor-default"
                    type="button">
                    <PlusIcon class="w-5 h-5" />
                </button></div>
        </div>
    </div>
</template>
<script setup>
import { PlusIcon, MinusIcon } from '@heroicons/vue/solid';

const emit = defineEmits(['amount'])

;

const amount = ref({

    adult:1,
    children: 0,
    infant: 0
})


const addAdult = () => {
    amount.value.adult++;
    emit('amount', amount.value);
}
const subAdult = () => {
    amount.value.adult--;
    if (amount.value.adult <= 1) {
        amount.value.adult = 1;
    }
    emit('amount', amount.value);
}
const addChild = () => {
    amount.value.children++;
    emit('amount', amount.value);
}
const addInfant = () => {
    amount.value.infant++
    
    emit('amount', amount.value);
}
const subChild = () => {
    amount.value.children--;
    if (amount.value.children <= 0) {
        amount.value.children = 0;
    }
    emit('amount', amount.value);
}
const subInfant = () => {
    amount.value.infant--;
    if (amount.value.infant <= 0) {
        amount.value.infant = 0;
    }
    emit('amount', amount.value);
}
</script>