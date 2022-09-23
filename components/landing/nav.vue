<template>
    <nav class="fixed top-0 left-0 z-50 py-2 w-full bg-gray-50">
        <div class="py-3 px-4 lg:px-6">
            <div class="flex justify-between items-center">
                <div class="flex justify-start items-center">
                    <a href="#" class="text-md font-semibold flex items-center lg:mr-1.5">
                        <img src="/img/1.png" class="mr-2 h-6" alt="Winster Logo" />
                        <span class="self-center text-xl font-bold whitespace-nowrap">YoPress
                            <span class="hidden md:inline">Website Builder</span></span>
                    </a>
                    <div class="hidden md:flex md:ml-6">
                        <ul class="flex space-x-2 md:space-x-8">
                            <li>
                                <a href="#" class="
                      text-sm
                      font-medium
                      text-gray-700
                      hover:text-fuchsia-500
                    " aria-current="page">Home</a>
                            </li>
                            <li>
                                <a href="#" class="
                      text-sm
                      font-medium
                      text-gray-700
                      hover:text-fuchsia-500
                    " aria-current="page">Team</a>
                            </li>
                            <li>
                                <a href="#" class="
                      text-sm
                      font-medium
                      text-gray-700
                      hover:text-fuchsia-500
                    " aria-current="page">Pricing</a>
                            </li>
                            <li>
                                <a href="#" class="
                      text-sm
                      font-medium
                      text-gray-700
                      hover:text-fuchsia-500
                    " aria-current="page">Contact</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <a href="#" class="
                text-white
                bg-gradient-to-br
                from-pink-500
                to-violet-500
                hover:scale-[1.02]
                shadow-md shadow-gray-300
                transition-transform
                font-medium
                rounded-lg
                text-sm
                px-5
                py-2.5
                text-center
                inline-flex
                items-center
                mr-3
              ">
                        <MenuIcon class="mr-2 -ml-1 w-5 h-5" />
                        Login/Register
                    </a>
                    <button @click="showNav = !showNav" type="button" class="
                inline-flex
                justify-center
                items-center
                ml-3
                text-gray-400
                rounded-2xl
                md:hidden
                hover:text-gray-900
                focus:outline-none focus:ring-2 focus:ring-fuchsia-200
              ">
                        <MenuIcon class="w-6 h-6" />
                    </button>
                </div>
            </div>
        </div>
        <div v-if="showNav" class="block md:hidden">
            <ul class="pt-2">
                <li>
                    <a href="#" class="
                block
                py-2
                pr-4
                pl-3
                text-base
                font-normal
                text-gray-900
                bg-gray-100
              ">Dashboard</a>
                </li>
                <li>
                    <a href="#" class="
                block
                py-2
                px-3
                text-base
                font-normal
                text-gray-600
                border-b border-gray-100
                hover:bg-gray-50 hover:border-gray-300 hover:text-gray-900
              ">Team</a>
                </li>
                <li>
                    <a href="#" class="
                block
                py-2
                px-3
                text-base
                font-normal
                text-gray-600
                border-b border-gray-100
                hover:bg-gray-50 hover:border-gray-300 hover:text-gray-900
              ">Projects</a>
                </li>
                <li>
                    <a href="#" class="
                block
                py-2
                px-3
                text-base
                font-normal
                text-gray-600
                border-b border-gray-100
                hover:bg-gray-50 hover:border-gray-300 hover:text-gray-900
              ">Calendar
                    </a>
                </li>
                <li class="block">
                    <a href="#" class="
                inline-flex
                items-center
                px-3
                pt-2
                text-base
                font-normal
                text-gray-600
                hover:bg-gray-50 hover:border-gray-300 hover:text-gray-900
              ">
                        <svg class="mr-2 w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"
                            xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M11 16l-4-4m0 0l4-4m-4 4h14m-5 4v1a3 3 0 01-3 3H6a3 3 0 01-3-3V7a3 3 0 013-3h7a3 3 0 013 3v1">
                            </path>
                        </svg>
                        Login/Register
                    </a>
                </li>
            </ul>
        </div>
    </nav>

</template>
<script setup>
import { ref } from "vue";
import { MenuIcon, XIcon } from "@heroicons/vue/outline";

const showNav = ref(false);
</script>