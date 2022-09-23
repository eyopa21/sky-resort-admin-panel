<template>
  <div class="nc-SectionHero2 relative" data-nc-id="SectionHero2">
    <div class="absolute inset-y-0 w-5/6 xl:w-3/4 right-0 flex-grow">
      <img
        class="absolute inset-0 object-cover w-full h-full opacity-30"
        src="../../assets/img/unity.jpg"
        alt="hero"
      />
    </div>
    <div class="relative py-14 lg:py-20">
      <div class="relative inline-flex">
        <div
          class="w-screen right-20 md:right-52 inset-y-0 absolute bg-primary-500"
        ></div>
        <div
          class="relative max-w-3xl inline-flex flex-shrink-0 flex-col items-start py-16 sm:py-20 lg:py-24 space-y-8 sm:space-y-10 text-white"
        >
          <h2
            class="font-semibold text-4xl md:text-5xl xl:text-7xl !leading-[110%]"
          >
            Welcome to <br />
            Sky resort and spa
          </h2>
        </div>
      </div>
      <div class="hidden lg:block lg:mt-20 w-full">
        <div
          class="nc-HeroRealEstateSearchForm w-full max-w-6xl py-5 lg:py-0"
          data-nc-id="HeroRealEstateSearchForm"
        >
          <form
            @submit.prevent="search()"
            class="w-full relative xl:mt-8 flex flex-col lg:flex-row lg:items-center rounded-3xl lg:rounded-full shadow-xl dark:shadow-2xl bg-white dark:bg-neutral-800 divide-y divide-neutral-200 dark:divide-neutral-700 lg:divide-y-0"
          >
            <div class="relative flex flex-[1.5]">
              <div
                class="flex flex-1 relative [ nc-hero-field-padding ] flex-shrink-0 items-center space-x-3 cursor-pointer focus:outline-none text-left text-white"
              >
                <div class="text-neutral-300 dark:text-neutral-400">
                  <LocationMarkerIcon class="nc-icon-field" />
                </div>
                <div class="flex-grow text-white">
                  <input
                    name="checkin"
                    type="date"
                    class="block w-48 bg-transparent border-none focus:ring-0 p-0 focus:outline-none focus:placeholder-neutral-300 xl:text-lg font-semibold placeholder-white dark:placeholder-neutral-200 truncate"
                    placeholder="Sep 2"
                    v-model="value"
                  />

                  <span
                    class="mt-0.5 text-sm text-neutral-400 font-light flex flex-row"
                    ><ExclamationIcon
                      v-if="errorMessage"
                      class="w-6 h-6 animate-bounce text-red-500"
                    /><span class="line-clamp-1">Check In? </span>
                  </span>
                </div>
              </div>
            </div>
            <div class="flex relative flex-1">
              <button
                class="flex text-left w-full flex-shrink-0 items-center [ nc-hero-field-padding ] space-x-3 focus:outline-none cursor-pointer"
                id="headlessui-popover-button-:rao:"
                type="button"
              >
                <div class="text-neutral-300 dark:text-neutral-400">
                  <LocationMarkerIcon class="nc-icon-field nc-icon-field-2" />
                </div>
                <div class="flex-grow text-white">
                  <input
                    type="date"
                    class="block w-full bg-transparent border-none focus:ring-0 p-0 focus:outline-none focus:placeholder-neutral-300 xl:text-lg font-semibold placeholder-white dark:placeholder-neutral-200 truncate"
                    placeholder="dd-mm-yyyy"
                    v-model="checkOutValue"
                  />

                  <span class="flex flex-row mt-0.5 text-sm text-neutral-400 font-light"
                    ><ExclamationIcon
                    v-if="checkOutError"
                    class="w-6 h-6 animate-bounce text-red-500"
                  /><span class="line-clamp-1">Check out?</span></span
                  >
                </div>
              </button>
            </div>
            <div class="flex relative flex-[1.3]">
              <div
                class="flex-1 flex items-center focus:outline-none cursor-pointer"
              >
                <button
                  @click="showFilters = !showFilters"
                  class="flex-1 flex text-left items-center focus:outline-none [ nc-hero-field-padding ] space-x-3"
                  id="headlessui-popover-button-:rar:"
                  type="button"
                  aria-expanded="false"
                >
                  <div class="text-neutral-300 dark:text-neutral-400">
                    <LocationMarkerIcon class="nc-icon-field nc-icon-field-2" />
                  </div>
                  <div class="flex-grow">
                    <span class="block xl:text-lg font-semibold truncate"
                      >{{amount.adult}} adult</span
                    ><span
                      class="block mt-1 text-sm text-neutral-400 leading-none font-light"
                      >{{amount.children}} child, {{amount.infant}} infant</span
                    >
                  </div>
                </button>
                <VueFilters v-if="showFilters" @amount="(n) => (amount = n)"/>
                <div class="pr-2 xl:pr-4">
                  <button
                    type="submit"
                    class="h-14 md:h-16 w-full md:w-16 rounded-full bg-primary-6000 hover:bg-primary-700 flex items-center justify-center text-neutral-50 focus:outline-none"
                  >
                    <span class="mr-3 md:hidden">Search</span>
                    <SearchIcon class="h-6 w-6" />
                  </button>
                </div>
              </div>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import {
  LocationMarkerIcon,
  SearchIcon,
  ExclamationIcon,
} from "@heroicons/vue/solid";
import { useForm, useField } from "vee-validate";
const { handleSubmit } = useForm();

const amount = ref({

adult:1,
children: 0,
infant: 0
})


const { value, errorMessage } = useField("checkin", "required");
const { value:checkOutValue, errorMessage:checkOutError } = useField("checkout", "required");

const search = handleSubmit((formValues) => {
  console.log(formValues);
  console.log(amount.value)
});

const showFilters = ref(false);
const showCalendar = ref(false);
</script>
