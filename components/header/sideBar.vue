<template>
    <div @click="layout.showSideBar=false" class="relative z-50 overflow-hidden"  >
        <div class="fixed inset-0 bg-slate-900 bg-opacity-50 opacity-100" ></div>
        <div class="fixed inset-0">
            <div class="flex justify-end min-h-full">
                <div class="w-full max-w-md overflow-hidden transition-all opacity-100 translate-x-0"
                    id="headlessui-dialog-panel-:r3b:">
                    <div
                        class="overflow-y-auto w-full h-screen py-2 transition transform shadow-lg ring-1 dark:ring-neutral-700 bg-white dark:bg-neutral-900 divide-y-2 divide-neutral-100 dark:divide-neutral-800">
                        <div class="py-6 px-5">
                            <a class="ttnc-logo inline-block text-primary-6000 focus:outline-none focus:ring-0 w-24"
                                href="/chisfis/" tabindex="0">
                                <div class="w-full hidden dark:block">logo</div>
                            </a>
                            <div class="flex flex-col mt-5 text-neutral-700 dark:text-neutral-300 text-sm">
                                <span>Reserve a room now using your phone only!!</span>
                                <div class="flex justify-between items-center mt-4">
                                    <nav class="nc-SocialsList flex space-x-2.5 text-2xl text-neutral-6000 dark:text-neutral-300"
                                        data-nc-id="SocialsList">
                                        <a class="w-9 h-9 flex items-center justify-center rounded-full bg-neutral-100 text-xl dark:bg-neutral-800 dark:text-neutral-300"
                                            href="#" target="_blank" rel="noopener noreferrer" title="Facebook">fb</a><a
                                            class="w-9 h-9 flex items-center justify-center rounded-full bg-neutral-100 text-xl dark:bg-neutral-800 dark:text-neutral-300"
                                            href="#" target="_blank" rel="noopener noreferrer" title="Twitter">tw</a><a
                                            class="w-9 h-9 flex items-center justify-center rounded-full bg-neutral-100 text-xl dark:bg-neutral-800 dark:text-neutral-300"
                                            href="#" target="_blank" rel="noopener noreferrer" title="Youtube">yt</a><a
                                            class="w-9 h-9 flex items-center justify-center rounded-full bg-neutral-100 text-xl dark:bg-neutral-800 dark:text-neutral-300"
                                            href="#" target="_blank" rel="noopener noreferrer" title="Instagram">it</a>
                                    </nav>
                                    <span class="block"><button
                                            class="text-2xl md:text-3xl w-12 h-12 rounded-full text-neutral-700 dark:text-neutral-300 hover:bg-neutral-100 dark:hover:bg-neutral-800 focus:outline-none flex items-center justify-center bg-neutral-100 dark:bg-neutral-800">
                                            <span class="sr-only">Enable dark mode</span>
                                            <MoonIcon class="w-7 h-7" />
                                        </button></span>
                                </div>
                            </div>
                            <span class="absolute right-2 top-2 p-1"><button @click="layout.showSideBar = false"
                                    class="w-8 h-8 flex items-center justify-center rounded-full text-neutral-700 dark:text-neutral-300 hover:bg-neutral-100 dark:hover:bg-neutral-700 focus:outline-none">
                                    <span class="sr-only">Close</span>
                                    <XIcon class="w-5 h-5" />
                                </button></span>
                        </div>
                        <ul class="flex flex-col py-6 px-2 space-y-1">
                            <li class="text-neutral-900 dark:text-white">
                                <NuxtLink
                                    class="flex w-full px-4 font-medium uppercase tracking-wide text-sm hover:bg-neutral-100 dark:hover:bg-neutral-800 rounded-lg"
                                    to="/"><span class="py-2.5 pr-3">Home</span><span class="flex-1 flex"><span
                                            class="py-2.5 flex items-center justify-end flex-1"
                                            id="headlessui-disclosure-button-:r3c:" aria-expanded="false">
                                            <HomeIcon class="ml-2 h-4 w-4" />
                                        </span></span></NuxtLink>
                            </li>

                            <li class="text-neutral-900 dark:text-white">
                                <NuxtLink
                                    class="flex w-full px-4 font-medium uppercase tracking-wide text-sm hover:bg-neutral-100 dark:hover:bg-neutral-800 rounded-lg"
                                    to="/rooms"><span class="py-2.5 pr-3">Rooms</span><span class="flex-1 flex"><span
                                            class="py-2.5 flex items-center justify-end flex-1"
                                            id="headlessui-disclosure-button-:r3c:" aria-expanded="false">
                                            <OfficeBuildingIcon class="ml-2 h-4 w-4" />
                                        </span></span></NuxtLink>
                            </li>
                            <li class="text-neutral-900 dark:text-white">
                                <NuxtLink
                                    class="flex w-full px-4 font-medium uppercase tracking-wide text-sm hover:bg-neutral-100 dark:hover:bg-neutral-800 rounded-lg"
                                    to="about"><span class="py-2.5 pr-3">About</span><span class="flex-1 flex"><span
                                            class="py-2.5 flex items-center justify-end flex-1"
                                            id="headlessui-disclosure-button-:r3c:" aria-expanded="false">
                                            <IdentificationIcon class="ml-2 h-4 w-4" />
                                        </span></span></NuxtLink>
                            </li>
                            <li class="text-neutral-900 dark:text-white">
                                <NuxtLink
                                    class="flex w-full px-4 font-medium uppercase tracking-wide text-sm hover:bg-neutral-100 dark:hover:bg-neutral-800 rounded-lg"
                                    to="/gallery"><span class="py-2.5 pr-3">Gallery</span><span
                                        class="flex-1 flex"><span class="py-2.5 flex items-center justify-end flex-1"
                                            id="headlessui-disclosure-button-:r3c:" aria-expanded="false">
                                            <PhotographIcon class="ml-2 h-4 w-4" />
                                        </span></span></NuxtLink>
                            </li>
                            <li class="text-neutral-900 dark:text-white">
                                <NuxtLink
                                    class="flex w-full px-4 font-medium uppercase tracking-wide text-sm hover:bg-neutral-100 dark:hover:bg-neutral-800 rounded-lg"
                                    to="/contact"><span class="py-2.5 pr-3">Home</span><span class="flex-1 flex"><span
                                            class="py-2.5 flex items-center justify-end flex-1"
                                            id="headlessui-disclosure-button-:r3c:" aria-expanded="false">
                                            <PhoneIcon class="ml-2 h-4 w-4" />
                                        </span></span></NuxtLink>
                            </li>
                        </ul>
                        <div class="flex items-center justify-between py-6 px-5">
                            <NuxtLink class="inline-block" to="/rooms" rel="noopener noreferrer"><button
                                    class="nc-Button relative h-auto inline-flex items-center justify-center rounded-full transition-colors text-sm sm:text-base font-medium px-4 py-3 sm:px-6 ttnc-ButtonPrimary disabled:bg-opacity-70 bg-primary-6000 hover:bg-primary-700 text-neutral-50 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-primary-6000 dark:focus:ring-offset-0">
                                    Reserve a room
                                </button></NuxtLink>
                            <!--div class="LangDropdown">
                <div class="relative">
                  <button
                    class="text-opacity-80 group px-3 py-1.5 border-neutral-300 hover:border-neutral-400 dark:border-neutral-700 rounded-full inline-flex items-center text-sm text-gray-700 dark:text-neutral-300 font-medium hover:text-opacity-100 focus:outline-none focus-visible:ring-2 focus-visible:ring-white focus-visible:ring-opacity-75"
                    id="headlessui-popover-button-:r3m:"
                    type="button"
                    aria-expanded="false"
                  >
                   <GlobeAltIcon   class="w-[18px] h-[18px] opacity-80"/> <span class="ml-2 select-none">Language</span
                    >
                    <ChevronDownIcon class="text-opacity-70 ml-2 h-4 w-4 group-hover:text-opacity-80 transition ease-in-out duration-150"/>
                  </button>
                </div>
              </div-->
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import {
    XIcon, MoonIcon, GlobeAltIcon,
    MenuIcon,

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
