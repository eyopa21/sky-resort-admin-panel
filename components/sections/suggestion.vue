<template>
    <div class="nc-SectionSliderNewCategories ">
        <div
            class="SectionSliderNewCategories__PageHome2_s1nc__rb6_ flow-root glide--ltr glide--slider glide--swipeable">
            <div
                class="nc-Section-Heading relative flex flex-col sm:flex-row sm:items-end justify-between mb-12 lg:mb-16 text-neutral-900 dark:text-neutral-50">
                <div class="max-w-2xl">
                    <h2 class="text-3xl md:text-4xl font-semibold">Suggestions for discovery</h2><span
                        class="mt-2 md:mt-3 font-normal block text-base sm:text-xl text-neutral-500 dark:text-neutral-400">Popular
                        places to stay that Chisfis recommends for you</span>
                </div>
                <!--div class="mt-4 flex justify-end sm:ml-2 sm:mt-0 flex-shrink-0">
                    <div class="nc-NextPrev relative flex items-center text-neutral-900 dark:text-neutral-300 "
                        data-nc-id="NextPrev" data-glide-el="controls"><button
                            class="w-10 h-10 mr-[6px] bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-6000 dark:hover:border-neutral-500 rounded-full flex items-center justify-center hover:border-neutral-300 focus:outline-none"
                            title="Prev" data-glide-dir="<"><i
                                class="las la-angle-left"></i></button><button
                            class="w-10 h-10 bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-6000 dark:hover:border-neutral-500 rounded-full flex items-center justify-center hover:border-neutral-300 focus:outline-none"
                            title="Next" data-glide-dir=">"><i class="las la-angle-right"></i></button>
                    </div>
                </div-->
            </div>
            <div class="glide__track overflow-x-scroll overflow-y-hidden" >
                <ul class="glide__slides "
                    style="transition: transform 0ms cubic-bezier(0.165, 0.84, 0.44, 1) 0s; width: 2525px; transform: translate3d(0px, 0px, 0px);">
                    <li v-for="card in cards" :key="card" class="glide__slide glide__slide--active "
                        style="width: 485px; margin-right: 10px;"><a
                            class="nc-CardCategory4 flex flex-col " 
                            href="/chisfis/listing-stay">
                            <div
                                class="flex-shrink-0 relative w-full aspect-w-5 aspect-h-4 sm:aspect-h-6 rounded-2xl overflow-hidden group">
                                <div class="nc-NcImage " >
                                    <div
                                        class="object-cover w-full h-72  rounded-2xl flex items-center justify-center bg-neutral-200 dark:bg-neutral-6000 text-neutral-100 dark:text-neutral-500">
                                        <div class="h-full w-full">
                                            <img class="h-full w-full" :src="card.image" alt="slide image">
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="-pt-32 -mt-64 px-2 truncate text-center">
                                <h2
                                    class="text-base sm:text-lg text-neutral-900 dark:text-neutral-100 font-medium truncate">
                                    Enjoy the great cold</h2><span
                                    class="block mt-2 text-sm text-neutral-6000 dark:text-neutral-400">188,288
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