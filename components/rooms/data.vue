<template>


    <div id="root">
        <div class="bg-slate-900 text-base  text-neutral-900 dark:text-neutral-200">


            <div class="h-1 absolute invisible"></div>
            <div class="ListingDetailPage nc-ListingStayDetailPage ">
                <header class="container 2xl:px-14 rounded-md sm:rounded-xl">
                    <div class="relative grid grid-cols-3 sm:grid-cols-4 gap-1 sm:gap-2">
                        <div
                            class="col-span-2 row-span-3 sm:row-span-2 relative rounded-md sm:rounded-xl overflow-hidden cursor-pointer">
                            <div class="nc-NcImage absolute inset-0" ><img
                                    src="https://images.pexels.com/photos/6129967/pexels-photo-6129967.jpeg?auto=compress&amp;cs=tinysrgb&amp;dpr=3&amp;h=750&amp;w=1260"
                                    class="object-cover w-full h-full rounded-md sm:rounded-xl" alt="nc-imgs"></div>
                            <div
                                class="absolute inset-0 bg-neutral-900 bg-opacity-20 opacity-0 hover:opacity-100 transition-opacity">
                            </div>
                        </div>
                        <div class="relative rounded-md sm:rounded-xl overflow-hidden ">
                            <div class="nc-NcImage aspect-w-4 aspect-h-3 sm:aspect-w-6 sm:aspect-h-5"
                                ><img
                                    src="https://images.pexels.com/photos/7163619/pexels-photo-7163619.jpeg?auto=compress&amp;cs=tinysrgb&amp;dpr=2&amp;h=750&amp;w=1260"
                                    class="object-cover w-full h-full rounded-md sm:rounded-xl " alt="nc-imgs">
                            </div>
                            <div
                                class="absolute inset-0 bg-neutral-900 bg-opacity-20 opacity-0 hover:opacity-100 transition-opacity cursor-pointer">
                            </div>
                        </div>
                        <div class="relative rounded-md sm:rounded-xl overflow-hidden ">
                            <div class="nc-NcImage aspect-w-4 aspect-h-3 sm:aspect-w-6 sm:aspect-h-5"
                                data-nc-id="NcImage"><img
                                    src="https://images.pexels.com/photos/6527036/pexels-photo-6527036.jpeg?auto=compress&amp;cs=tinysrgb&amp;dpr=2&amp;h=750&amp;w=1260"
                                    class="object-cover w-full h-full rounded-md sm:rounded-xl " alt="nc-imgs">
                            </div>
                            <div
                                class="absolute inset-0 bg-neutral-900 bg-opacity-20 opacity-0 hover:opacity-100 transition-opacity cursor-pointer">
                            </div>
                        </div>
                        <div class="relative rounded-md sm:rounded-xl overflow-hidden ">
                            <div class="nc-NcImage aspect-w-4 aspect-h-3 sm:aspect-w-6 sm:aspect-h-5"
                                data-nc-id="NcImage"><img
                                    src="https://images.pexels.com/photos/6969831/pexels-photo-6969831.jpeg?auto=compress&amp;cs=tinysrgb&amp;dpr=2&amp;h=750&amp;w=1260"
                                    class="object-cover w-full h-full rounded-md sm:rounded-xl " alt="nc-imgs">
                            </div>
                            <div
                                class="absolute inset-0 bg-neutral-900 bg-opacity-20 opacity-0 hover:opacity-100 transition-opacity cursor-pointer">
                            </div>
                        </div>
                        <div class="relative rounded-md sm:rounded-xl overflow-hidden hidden sm:block">
                            <div class="nc-NcImage aspect-w-4 aspect-h-3 sm:aspect-w-6 sm:aspect-h-5"
                                data-nc-id="NcImage"><img
                                    src="https://images.pexels.com/photos/6438752/pexels-photo-6438752.jpeg?auto=compress&amp;cs=tinysrgb&amp;dpr=2&amp;h=750&amp;w=1260"
                                    class="object-cover w-full h-full rounded-md sm:rounded-xl " alt="nc-imgs">
                            </div>
                            <div
                                class="absolute inset-0 bg-neutral-900 bg-opacity-20 opacity-0 hover:opacity-100 transition-opacity cursor-pointer">
                            </div>
                        </div>
                        <button
                            @click="layout.showImages = true"
                            class="absolute flex md:items-center md:justify-center left-3 bottom-3 px-4 py-1 md:py-2 rounded-xl bg-neutral-100 text-neutral-500 cursor-pointer hover:bg-neutral-200 z-10">
                            <MenuIcon class="w-5 h-5" />
                            <span class="ml-2 text-neutral-800 text-sm font-medium">Show all photos</span>
                        </button>
                        <div v-if="layout.showImages">
                            
                            <RoomsAllImages/>
                        </div>
                    </div>
                </header>
                <div
                    style="position: absolute; width: 1px; height: 1px; padding: 0px; margin: -1px; overflow: hidden; clip: rect(0px, 0px, 0px, 0px); white-space: nowrap; border-width: 0px; display: none;">
                </div>
                <main class="container relative z-10 mt-11 flex flex-col lg:flex-row ">
                    <div class="w-full lg:w-3/5 xl:w-2/3 space-y-8 lg:space-y-10 lg:pr-10">
                        <div class="listingSection__wrap !space-y-6">
                            <div class="flex justify-between items-center"><span
                                    class="nc-Badge inline-flex px-2.5 py-1 rounded-full font-medium text-xs  text-blue-800 bg-blue-100  relative">premium</span>
                                <div class="flow-root">
                                    <div class="flex text-neutral-700 dark:text-neutral-300 text-sm -mx-3 -my-1.5">
                                        <span
                                            class="py-1.5 px-3 flex rounded-lg hover:bg-neutral-100 dark:hover:bg-neutral-800 cursor-pointer">
                                            
                                            <ShareIcon class="w-5 h-5"/>
                                            <span class="hidden sm:block ml-2.5">Share</span></span><span
                                            class="py-1.5 px-3 flex rounded-lg hover:bg-neutral-100 dark:hover:bg-neutral-800 cursor-pointer">
                                            <ThumbUpIcon class="w-5 h-5"/>
                                            <span class="hidden sm:block ml-2.5">Save</span></span>
                                    </div>
                                </div>
                            </div>
                            <h2 class="text-2xl sm:text-3xl lg:text-4xl font-semibold">Deluxe room
                            </h2>
                            <div class="flex items-center space-x-4">
                                <div class="nc-StartRating flex items-center space-x-1 text-sm  "
                                    data-nc-id="StartRating">
                                    <div class="pb-[2px]">
                                    <StarIcon  class="w-[18px] h-[18px] text-orange-500"/>
                                    </div><span class="font-medium ">4.5</span><span
                                        class="text-neutral-500 dark:text-neutral-400">(112)</span>
                                </div><span>·</span><span class="flex flex-row">Views: <span class="ml-1">
                                        Lake tana, the pool</span></span>
                            </div>
                            <div class="flex items-center">
                                <div class="">
                                    
                                    Bed type:
                                </div>
                                <span class="ml-2.5 text-neutral-500 dark:text-neutral-400">Queen bed, Sofa</span>
                            </div>
                            <div class="w-full border-b border-neutral-100 dark:border-neutral-700"></div>
                            <div
                                class="flex items-center justify-between xl:justify-start space-x-8 xl:space-x-12 text-sm text-neutral-700 dark:text-neutral-300">
                                <div class="flex items-center space-x-3 "><UsersIcon class="w-4 h-4" /><span
                                        class="">6 <span class="hidden sm:inline-block">guests</span></span></div>
                                <div class="flex items-center space-x-3"><InboxIcon class="w-4 h-4" /><span
                                        class=" ">6 <span class="hidden sm:inline-block">beds</span></span></div>
                                <div class="flex items-center space-x-3"><ReceiptTaxIcon class="w-4 h-4" /><span
                                        class=" ">3 <span class="hidden sm:inline-block">baths</span></span></div>
                                <div class="flex items-center space-x-3"> <ArrowsExpandIcon class="w-4 h-4" /> <span
                                        ><span class="hidden sm:inline-block">40m<sup>2</sup></span></span></div>
                            </div>
                        </div>
                        <RoomsDataRoomInfo />
                        <RoomsDataFeatures />

                        <RoomsDataRoomRates />

                        <RoomsDataRefundPolicy />
                    </div>
                    <RoomsReserve />
                </main>
                <RoomsBottomButton />
                <div class="container py-24 lg:py-32">
                   <SectionsRecommendation/>
                    <SectionsContact class="mt-32"/>
                </div>
            </div>

        </div>
    </div>



</template>

<script setup>
import {
  ChevronLeftIcon,
  ChevronRightIcon,
  UserIcon,
  UsersIcon,
  InboxIcon,
  ReceiptTaxIcon,
  ArrowsExpandIcon,
  StarIcon,
  CurrencyDollarIcon,
  ThumbUpIcon,
  ShareIcon,
  ViewBoardsIcon, 
  MenuIcon,
  EyeIcon
} from "@heroicons/vue/solid";
const layout = useLayout()
</script>