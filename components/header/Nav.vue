<template>
    <div
        class="nc-Header bsticky top-0 w-full left-0 right-0 z-40 nc-header-bg shadow-sm border-b border-slate-700">
        <div class="nc-MainNav1 nc-MainNav2 relative z-10 bg-slate-900">
            <div class="px-4 lg:container py-4 lg:py-5 relative flex justify-between items-center">
                <div class="hidden  md:flex justify-start flex-1 items-center space-x-3 sm:space-x-8 lg:space-x-10">
                    <a class="ttnc-logo inline-block text-primary-6000 focus:outline-none focus:ring-0 w-24"
                        href="/chisfis/">logo</a>
                    <div class="hidden lg:block h-10 border-l border-neutral-300 dark:border-neutral-500"></div>
                    <div class="hidden lg:block">
                        <div class="DropdownTravelers">
                            <div class="relative">
                                <NuxtLink to="/"
                                    class="text-opacity-90 group py-2 rounded-md text-sm sm:text-base font-medium hover:text-opacity-100 focus:outline-none focus-visible:ring-2 focus-visible:ring-white focus-visible:ring-opacity-75"
                                    id="headlessui-popover-button-:rb8:" type="button" aria-expanded="false">
                                    <div class="inline-flex items-center hover:scale-110" role="button">
                                        <HomeIcon class="w-[18px] h-[18px] opacity-80 mr-1" />
                                        <span>Home</span>


                                    </div>
                                </NuxtLink>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="lg:hidden flex-[3] max-w-lg !mx-auto md:px-3">
                    <div class="HeroSearchForm2RealEstateMobile">
                        <button
                            class="relative flex items-center w-full border border-neutral-200 dark:border-neutral-6000 px-4 py-2 pr-11 rounded-full shadow-lg">
                            <SearchIcon class="flex-shrink-0 w-5 h-5" />
                            <div class="ml-3 flex-1 text-left overflow-hidden">
                                <span class="block font-medium text-sm">Where to?</span><span
                                    class="block mt-0.5 text-xs font-light text-neutral-500 dark:text-neutral-400 line-clamp-1">Anywhere
                                    • Any week • Add guests</span>
                            </div>
                            <span
                                class="absolute right-2 top-1/2 transform -translate-y-1/2 w-9 h-9 flex items-center justify-center rounded-full border border-neutral-200 dark:border-neutral-6000 dark:text-neutral-300">
                                <AdjustmentsIcon class="block w-4 h-4" />
                            </span>
                        </button>
                    </div>
                </div>
                <div
                    class="hidden md:flex flex-shrink-0 items-center justify-end flex-1 lg:flex-none text-neutral-700 dark:text-neutral-100">
                    <div class="hidden items-center lg:flex space-x-1">
                        <div class="CurrencyDropdown">
                          <div class="relative">
                                <NuxtLink to="/rooms"
                                    class="text-opacity-80 group px-3 py-1.5 border-neutral-300 hover:border-neutral-400 dark:border-neutral-700 rounded-full inline-flex items-center text-sm text-gray-700 dark:text-neutral-300 font-medium hover:text-opacity-100 focus:outline-none focus-visible:ring-2 focus-visible:ring-white focus-visible:ring-opacity-75"
                                    id="headlessui-popover-button-:rbb:" type="button" aria-expanded="false">


                                    <OfficeBuildingIcon class="w-[18px] h-[18px] opacity-80" />

                                    <span class="ml-2 select-none">Rooms</span>


                                </NuxtLink>
                            </div>
                        </div>
                        <div class="LangDropdown">
                            <div class="relative">
                                <NuxtLink to="/about"
                                    class="text-opacity-80 group px-3 py-1.5 border-neutral-300 hover:border-neutral-400 dark:border-neutral-700 rounded-full inline-flex items-center text-sm text-gray-700 dark:text-neutral-300 font-medium hover:text-opacity-100 focus:outline-none focus-visible:ring-2 focus-visible:ring-white focus-visible:ring-opacity-75"
                                    id="headlessui-popover-button-:rbe:" type="button" aria-expanded="false">


                                    <IdentificationIcon class="w-[18px] h-[18px] opacity-80" />

                                    <span class="ml-2 select-none">About</span>

                                </NuxtLink>
                            </div>
                        </div>
                        <div class="LangDropdown">
                            <div class="relative">
                                <NuxtLink to="/contact"
                                    class="text-opacity-80 group px-3 py-1.5 border-neutral-300 hover:border-neutral-400 dark:border-neutral-700 rounded-full inline-flex items-center text-sm text-gray-700 dark:text-neutral-300 font-medium hover:text-opacity-100 focus:outline-none focus-visible:ring-2 focus-visible:ring-white focus-visible:ring-opacity-75"
                                    id="headlessui-popover-button-:rbe:" type="button" aria-expanded="false">


                                    <PhoneIcon class="w-[18px] h-[18px] opacity-80" />

                                    <span class="ml-2 select-none">Contact</span>

                                </NuxtLink>
                            </div>
                        </div>
                        <NuxtLink
                            class="text-opacity-90 group px-4 py-2 border border-neutral-300 hover:border-neutral-400 dark:border-neutral-700 rounded-full inline-flex items-center text-sm text-gray-700 dark:text-neutral-300 font-medium hover:text-opacity-100 focus:outline-none focus-visible:ring-2 focus-visible:ring-white focus-visible:ring-opacity-75"
                            to="/Gallery">
                            <PhotographIcon class="w-[18px] h-[18px] opacity-80 mr-2" />Gallery
                        </NuxtLink>
                        <div></div>
                        <button
                            class=" text-2xl md:text-3xl w-12 h-12 rounded-full text-neutral-700 dark:text-neutral-300 hover:bg-neutral-100 dark:hover:bg-neutral-800 focus:outline-none flex items-center justify-end">
                            <span class="sr-only">Enable dark mode</span>
                            <MoonIcon class="w-7 h-7" />
                        </button>


                    </div>
                    <div class="flex items-center space-x-2 lg:selection lg:hidden">


                        <button @click="layout.showSideBar = !layout.showSideBar"
                            class="focus:outline-none flex items-center justify-center p-2.5 rounded-lg text-neutral-700 dark:text-neutral-300">

                            <MenuIcon class="h-7 w-7" />
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import {
    MoonIcon,
    MenuIcon,
    XIcon,
    HomeIcon,
    UserIcon,
    PhoneIcon,
    SearchIcon,
    ChevronDownIcon,
    IdentificationIcon,
    OfficeBuildingIcon,
    PhotographIcon,
    AdjustmentsIcon
} from "@heroicons/vue/solid";

const layout = useLayout();
</script>
