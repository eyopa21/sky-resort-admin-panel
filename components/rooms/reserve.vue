<template>
    <div class="hidden lg:block flex-grow mt-14 lg:mt-0">
        <div class="sticky top-28">
            <div class="listingSectionSidebar__wrap shadow-xl">
                <div class="flex justify-between"><span
                        class="text-3xl font-semibold">$119<span
                            class="ml-1 text-base font-normal text-neutral-500 dark:text-neutral-400">/night</span></span>
                    <div class="nc-StartRating flex items-center space-x-1 text-sm  "
                        data-nc-id="StartRating">
                        <div class="pb-[2px]">
                        <StarIcon  class="w-[18px] h-[18px] text-orange-500"/>
                        </div><span class="font-medium ">4.5</span><span
                            class="text-neutral-500 dark:text-neutral-400">(112)</span>
                    </div>
                </div>
                <form
                    class="flex flex-col border border-neutral-200 dark:border-neutral-700 rounded-3xl ">
                    <div
                        class="StayDatesRangeInput relative flex z-10 nc-ListingStayDetailPage__stayDatesRangeInput flex-1 nc-date-not-focusedInput">
                       
                        <div
                            class="flex-1 grid grid-cols-2 relative divide-x divide-neutral-200 dark:divide-neutral-700 !grid-cols-1 sm:!grid-cols-2">
                            <div
                                class="relative flex p-3 items-center space-x-3 cursor-pointer  ">
                                <div class="text-neutral-300 dark:text-neutral-400">
                                <CalendarIcon class="nc-icon-field"/>
                                </div>
                                <div class="flex-1"><span
                                        class="block xl:text-lg font-semibold">24
                                        Sep</span><span
                                        class="block mt-1 text-sm text-neutral-400 leading-none font-light">Check
                                        in</span></div>
                            </div>
                            <div
                                class="relative flex p-3 items-center space-x-3 cursor-pointer  ">
                                <div class="text-neutral-300 dark:text-neutral-400"><CalendarIcon class="nc-icon-field"/></div>
                                <div class="flex-1"><span
                                        class="block xl:text-lg font-semibold">30
                                        Sep</span><span
                                        class="block mt-1 text-sm text-neutral-400 leading-none font-light">Check
                                        out</span></div>
                            </div>
                        </div>
                    </div>
                    <div class="w-full border-b border-neutral-200 dark:border-neutral-700">
                    </div>
                    <div class="flex relative nc-ListingStayDetailPage__guestsInput flex-1">
                        <div
                        @click="showFilter = !showFilter"
                            class="flex-1 flex items-center focus:outline-none cursor-pointer ">
                            <button
                           
                                class="flex-1 flex text-left items-center p-3 space-x-3 "
                                type="button"
                                >
                                <div class="text-neutral-300 dark:text-neutral-400"><UserAddIcon class="nc-icon-field"/></div>
                                <div class="flex-grow"><span
                                        class="block xl:text-lg font-semibold">3
                                        Guests</span><span
                                        class="block mt-1 text-sm text-neutral-400 leading-none font-light">Guests</span>
                                </div>
                            </button>
                            <div class="relative"></div>
                        </div>
                        <VueFilters v-if="showFilter"/>
                    </div>
                </form>
                <div class="flex flex-col space-y-4">
                    <div
                        class="flex justify-between text-neutral-6000 dark:text-neutral-300">
                        <span>$119 x 3 night</span><span>$357</span></div>
                    <div
                        class="flex justify-between text-neutral-6000 dark:text-neutral-300">
                        <span>Service charge</span><span>$0</span></div>
                    <div class="border-b border-neutral-200 dark:border-neutral-700"></div>
                    <div class="flex justify-between font-semibold">
                        <span>Total</span><span>$199</span></div>
                </div><a
                    class="nc-Button relative h-auto inline-flex items-center justify-center rounded-full transition-colors text-sm sm:text-base font-medium px-4 py-3 sm:px-6  ttnc-ButtonPrimary disabled:bg-opacity-70 bg-primary-6000 hover:bg-primary-700 text-neutral-50  focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-primary-6000 dark:focus:ring-offset-0 "
                    >Reserve</a>
            </div>
        </div>
    </div>
</template>

<script setup>
import { CalendarIcon, UserAddIcon, StarIcon, CurrencyDollarIcon, } from '@heroicons/vue/solid';
const showFilter = ref(false);
</script>