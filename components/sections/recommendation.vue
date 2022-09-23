<template>
    <div class="nc-SectionSliderNewCategories ">
        <div
            class="SectionSliderNewCategories__ListingStayDetailPage1nc__r38_ flow-root glide--ltr glide--slider glide--swipeable">
            <div
                class="nc-Section-Heading relative flex flex-col sm:flex-row sm:items-end justify-between mb-12 lg:mb-16 text-neutral-900 dark:text-neutral-50">
                <div class="text-center w-full max-w-2xl mx-auto">
                    <h2 class="text-3xl md:text-4xl font-semibold">Explore by types of
                        stays</h2><span
                        class="mt-2 md:mt-3 font-normal block text-base sm:text-xl text-neutral-500 dark:text-neutral-400">Explore
                        houses based on 10 types of stays</span>
                </div>
            </div>
            <div class="glide__track__slide " data-glide-el="track">
                <ul class="glide__slides  "
                    style="transition: transform 0ms cubic-bezier(0.165, 0.84, 0.44, 1) 0s; width: 1536px; transform: translate3d(0px, 0px, 0px);">
                    <li v-for="card in cards" :key="card" class="glide__slide glide__slide--active" style="width: 224px; margin-right: 16px;"><a
                            class="nc-CardCategory5 flex flex-col " data-nc-id="CardCategory5">
                            <div
                                class="flex-shrink-0 relative w-full aspect-w-4 aspect-h-3 h-0 rounded-2xl overflow-hidden group">
                                <div class="nc-NcImage ">
                                    <div
                                        class="object-cover w-full h-full rounded-2xl flex items-center justify-center bg-neutral-200 dark:bg-neutral-6000 text-neutral-100 dark:text-neutral-500">
                                        <div class="h-full w-full">

                                            <img class="w-full h-full" :src="card.image" alt="">
                                        </div>
                                    </div>
                                </div><span
                                    class="opacity-0 group-hover:opacity-100 absolute inset-0 bg-black bg-opacity-10 transition-opacity"></span>
                            </div>
                            <div class="mt-4 px-3 truncate">
                                <h2
                                    class="text-base sm:text-lg text-neutral-900 dark:text-neutral-100 font-medium truncate">
                                    Nature House</h2><span
                                    class="block mt-2 text-sm text-neutral-6000 dark:text-neutral-400">17,288
                                    properties</span>
                            </div>
                        </a></li>
                    
                </ul>
            </div>
           
               
        </div>
    </div>
</template>

<script setup>
import { ChevronLeftIcon, ChevronRightIcon } from '@heroicons/vue/solid';

    const cards = ref([{
        image: '../../assets/img/unity.jpg',
        title: 'Title',
        subtitle: 'Subtitle'
    },
    {
        image: '../../assets/img/person.jpg',
        title: 'Title',
        subtitle: 'Subtitle'
    },
    {
        image: '../../assets/img/unity.jpg',
        title: 'Title',
        subtitle: 'Subtitle'
    },
    {
        image: '../../assets/img/person.jpg',
        title: 'Title',
        subtitle: 'Subtitle'
    },
    {
        image: '../../assets/img/unity.jpg',
        title: 'Title',
        subtitle: 'Subtitle'
    },
    {
        image: '../../assets/img/person.jpg',
        title: 'Title',
        subtitle: 'Subtitle'
    }])
</script>