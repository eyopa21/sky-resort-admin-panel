<template>
   <a href="#" class="flex py-3 px-4 border-b hover:bg-gray-100">
             <div class="flex-shrink-0">
                    <img
                      class="w-11 h-11 rounded-full"
                      src="/img/1.png"
                      alt="Jese image"
                    />
                    <div
                      class="
                        flex
                        absolute
                        justify-center
                        items-center
                        ml-6
                        -mt-5
                        w-5
                        h-5
                        bg-fuchsia-600
                        rounded-full
                        border border-white
                      "
                    >
                      <HomeIcon class="w-4 h-4"/>
                    </div>
                  </div>
                  <div class="pl-3 w-full">
                    <div class="text-gray-500 font-normal text-sm mb-1.5">
                      New message from
                      <span class="font-semibold text-gray-900"
                        >Bonnie Green</span
                      >: "Hey, what's up? All set for the presentation?"
                    </div>
                    <div class="text-xs font-medium text-fuchsia-500">
                      a few moments ago
                    </div>
                  </div>
                </a>
        

</template>
<script setup>
import { HomeIcon } from '@heroicons/vue/outline';

</script>