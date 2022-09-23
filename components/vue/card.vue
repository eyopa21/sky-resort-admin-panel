<template>
  <div
    class="nc-PropertyCardH group relative bg-gray-900 border border-neutral-100 dark:border-neutral-800 rounded-3xl overflow-hidden hover:shadow-xl transition-shadow h-full"
    data-nc-id="PropertyCardH"
  >
    <div class="h-full w-full flex flex-col sm:flex-row sm:items-center">
      <div class="flex-shrink-0 p-3 w-full sm:w-64">
        <div
          class="nc-GallerySlider w-full h-full rounded-2xl overflow-hidden will-change-transform"
          data-nc-id="GallerySlider"
        >
          <div
            class="gallerySlider__PropertyCardH_stayListing_0_nc__rau_ relative group overflow-hidden glide--ltr glide--slider glide--swipeable"
          >
            <div class="glide__track" >
              <ul
                class="glide__slides h-56"
                style="
                  transition: transform 0ms cubic-bezier(0.165, 0.84, 0.44, 1)
                    0s;
                  width: 1836px;
                  transform: translate3d(0px, 0px, 0px);
                "
              >
                <li
                  class=""
                  style="width: 459px; margin-right: 0px"
                >
                  <NuxtLink
                    class="block aspect-w-1 aspect-h-1"
                    to="/rooms/room"
                  >
                    <div class="nc-NcImage" data-nc-id="NcImage">
                      <img
                        :src="images[slide]"
                        class="object-cover w-full h-full"
                        alt="nc-imgs"
                      />
                    </div>
                  </NuxtLink>
                </li>
              </ul>
            </div>
            <div
              class="absolute -bottom-4 inset-x-0 h-10 bg-gradient-to-t from-neutral-900"
            ></div>
            <div
              class="glide__bullets flex items-center justify-center absolute bottom-2 left-1/2 transform -translate-x-1/2 space-x-1.5"
              data-glide-el="controls[nav]"
            >
              <div v-for="(url, key) in images" :key="key">
                <button
                  :class="
                    slide == key ? 'glide__bullet--active' : 'glide__bullet'
                  "
                  class="w-1.5 h-1.5 rounded-full bg-neutral-300"
                  @click="slide = key"
                ></button>
              </div>
            </div>
            <div
              class="absolute opacity-0 group-hover:opacity-100 transition-opacity flex top-1/2 transform -translate-y-1/2 inset-x-2 justify-between"
            >
              <div
                class="nc-NextPrev relative flex items-center text-neutral-900 dark:text-neutral-300 w-full justify-between"
              >
                <button
                  class="w-8 h-8 mr-[6px] bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-6000 dark:hover:border-neutral-500 rounded-full flex items-center justify-center hover:border-neutral-300 focus:outline-none"
                  @click="prev()"
                >
                  <ChevronLeftIcon class="w-4 h-4" /></button
                ><button
                  @click="next()"
                  class="w-8 h-8 bg-white dark:bg-neutral-900 border border-neutral-200 dark:border-neutral-6000 dark:hover:border-neutral-500 rounded-full flex items-center justify-center hover:border-neutral-300 focus:outline-none"
                >
                  <ChevronRightIcon class="w-4 h-4" />
                </button>
              </div>
            </div>
          </div>
        </div>
        <div
          class="nc-SaleOffBadge flex items-center justify-center text-xs py-0.5 px-3 text-red-50 rounded-full absolute left-5 top-5 !bg-orange-500"
          data-nc-id="SaleOffBadge"
        >
          -10% today
        </div>
      </div>
      <NuxtLink
        to="/rooms/room"
        class="flex-grow p-3 sm:pr-6 flex flex-col items-start"
      >
        <div class="space-y-4 w-full">
          <div class="inline-flex space-x-3">
            <span
              class="nc-Badge inline-flex px-2.5 py-1 rounded-full font-medium text-xs relative text-blue-800 bg-blue-100"
            >
              <div class="flex items-center">
                <UserIcon class="w-3 h-3" />
                <span class="ml-1">4 People</span>
              </div> </span
            ><span
              class="nc-Badge inline-flex px-2.5 py-1 rounded-full font-medium text-xs relative text-yellow-800 bg-yellow-100"
            >
              <div class="flex items-center">
                <UsersIcon class="w-3 h-3" />
                <span class="ml-1">Family</span>
              </div>
            </span>
          </div>
          <div class="flex items-center space-x-2">
            <span
              class="nc-Badge inline-flex px-2.5 py-1 rounded-full font-medium text-xs text-green-800 bg-green-100 relative"
              >ADS</span
            >
            <h2 class="text-lg font-medium capitalize">
              <span class="line-clamp-2">Best Western Cedars Hotel </span>
            </h2>
          </div>
          <div class="inline-grid grid-cols-3 gap-2">
            <div class="flex items-center space-x-2">
              <span class="hidden sm:inline-block">
                <InboxIcon class="w-3 h-3" /></span
              ><span class="text-xs text-neutral-500 dark:text-neutral-400"
                >6 beds</span
              >
            </div>
            <div class="flex items-center space-x-2">
              <span class="hidden sm:inline-block">
                <ReceiptTaxIcon class="w-3 h-3" /></span
              ><span class="text-xs text-neutral-500 dark:text-neutral-400"
                >3 baths</span
              >
            </div>
            <div class="flex items-center space-x-2">
              <span class="hidden sm:inline-block">
                <ArrowsExpandIcon class="w-3 h-3" /> </span
              ><span class="text-xs text-neutral-500 dark:text-neutral-400"
                >1200 Sq. Fit</span
              >
            </div>
          </div>
          <div
            class="w-14 border-b border-neutral-100 dark:border-neutral-800"
          ></div>
          <div class="flex w-full justify-between items-end">
            <div
              class="nc-StartRating flex items-center space-x-1 text-sm"
              data-nc-id="StartRating"
            >
              <div class="pb-[2px]">
                <StarIcon class="w-[18px] h-[18px] text-orange-500" />
              </div>
              <span class="font-medium">4.8</span
              ><span class="text-neutral-500 dark:text-neutral-400">(28)</span>
            </div>
            <span
              class="flex items-center justify-center px-3 py-2 border border-secondary-500 rounded leading-none text-base font-medium text-secondary-500"
            >
              <CurrencyDollarIcon class="w-5 h-5" />26,000</span
            >
          </div>
        </div>
      </NuxtLink>
    </div>
    <div
      class="nc-BtnLikeIcon w-8 h-8 flex items-center justify-center rounded-full cursor-pointer bg-neutral-100 dark:bg-neutral-700 hover:bg-neutral-200 hover:bg-opacity-70 text-neutral-6000 dark:text-neutral-400 absolute right-5 top-5 sm:right-3 sm:top-3"
      data-nc-id="BtnLikeIcon"
      title="Save"
    >
      <ThumbUpIcon class="h-5 w-5" />
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
} from "@heroicons/vue/solid";
const slide = ref(0);
const images = ref([
  "../../assets/img/unity.jpg",
  "../../assets/img/person.jpg",
  "../../assets/img/unity.jpg",
  "../../assets/img/person.jpg",
]);
const next = () => {
  slide.value++;
  if (slide.value >= images.value.length) {
    slide.value = 0;
  }
};
const prev = () => {
  slide.value--;
  if (slide.value < 0) {
    slide.value = images.value.length - 1;
  }
};
</script>
