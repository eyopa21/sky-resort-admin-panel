<template>



    <div id="headlessui-portal-root">
        <div data-headlessui-portal=""><button type="button" aria-hidden="true"
                style="position: absolute; width: 1px; height: 1px; padding: 0px; margin: -1px; overflow: hidden; clip: rect(0px, 0px, 0px, 0px); white-space: nowrap; border-width: 0px;"></button>
            <div>
                <div class="ProductDetailModalPhotos fixed inset-0 z-50 overflow-y-auto dark bg-neutral-800 text-neutral-200 hiddenScrollbar"
                    id="headlessui-dialog-:r1r:" role="dialog" aria-modal="true">
                    <div class="min-h-screen px-4 text-center">
                        <div class="fixed inset-0 bg-white dark:bg-neutral-800" id="headlessui-dialog-overlay-:r22:"
                            aria-hidden="true"></div>
                        <div class="absolute left-2 top-2 md:top-4 md:left-4 z-50">
                            <button @click="layout.showImages = false"
                                class="w-8 h-8 flex items-center justify-center rounded-full text-neutral-700 dark:text-neutral-300 hover:bg-neutral-100 dark:hover:bg-neutral-700  sm:w-12 sm:h-12 focus:outline-none"><span
                                    class="sr-only">Close</span>
                                <XIcon class="w-5 h-5" />
                            </button>
                        </div>
                        
    <div class="relative inline-block w-full max-w-5xl py-5 sm:py-8 h-screen align-middle mx-auto">
        <div
            class="modalPhotos-single-gallery glidejs_r1q_ group relative flex flex-col z-50 w-full h-full glide--ltr glide--slider glide--swipeable">
            <div class="controls_nav glide__bullets mb-4" data-glide-el="controls[nav]">
                <div class="text-center hidden text-sm glide__bullet--active"><span class="text-xl font-semibold">
                        {{slide+1}}</span><span> / {{images.length}}</span></div>
                
            </div>
            <div class="flex justify-center glide__track max-h-full h-full relative z-50">
                <ul class="glide__slides h-full w-full"
                    style="transition: transform 0ms cubic-bezier(0.165, 0.84, 0.44, 1) 0s; width: 9306px; transform: translate3d(0px, 0px, 0px);">
                    <li class="glide__slide relative h-full glide__slide--active"
                        style="width: 1024px; margin-right: 5px;">
                        <div class="nc-NcImage  w-full h-full flex items-center justify-center " >
                            <img :src="images[slide]"
                                class=" max-w-full max-h-full rounded-2xl" alt="nc-imgs"></div>
                    </li>
                   
                </ul>
            </div>
            <div
                class="xl:absolute z-20 xl:-inset-x-20 max-w-6xl my-2 mx-auto top-full xl:top-1/2 transform xl:-translate-y-1/2 flex xl:justify-between glide__arrows">
                <div class="nc-NextPrev relative flex items-center text-neutral-900 dark:text-neutral-300 mr-1.5"
                    ><button
                    @click="prev()"
                        class="w-8 h-8 sm:w-10 sm:h-10   bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-6000 dark:hover:border-neutral-500 rounded-full flex items-center justify-center hover:border-neutral-300 focus:outline-none"
                        ><ChevronLeftIcon class="w-5 h-5"/></button></div>
                <div class="nc-NextPrev relative flex items-center text-neutral-900 dark:text-neutral-300 ml-1.5"
                   ><button
                   @click="next()"
                        class="w-8 h-8 sm:w-10 sm:h-10  bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-6000 dark:hover:border-neutral-500 rounded-full flex items-center justify-center hover:border-neutral-300 focus:outline-none"
                       ><ChevronRightIcon class="w-5 h-5"/></button></div>
            </div>
        </div>
    </div>
                    </div>
                </div>
            </div><button type="button" aria-hidden="true"
                style="position: absolute; width: 1px; height: 1px; padding: 0px; margin: -1px; overflow: hidden; clip: rect(0px, 0px, 0px, 0px); white-space: nowrap; border-width: 0px;"></button>
        </div>
    </div>

</template>

<script setup>
import { ChevronLeftIcon, ChevronRightIcon, XIcon } from '@heroicons/vue/solid';
const slide = ref(0);
const next = () => {
  slide.value++;
  if (slide.value >=images.value.length) {
    slide.value = 0;
  }
};
const prev = () => {
  slide.value--;
  if (slide.value < 0) {
    slide.value = images.value.length - 1;
  }
};

const images = ref([
  "../../assets/img/unity.jpg",
  "../../assets/img/person.jpg",
  "../../assets/img/unity.jpg",
  "../../assets/img/person.jpg",
]);

const layout = useLayout();
</script>