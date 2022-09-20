<template>
 <div
          class="
            grid grid-cols-1
            gap-6
            mb-6
            w-full
            md:grid-cols-2
            xl:grid-cols-4
          "
        >
          <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4">
            <div class="flex items-center">
              <div
                class="
                  inline-flex
                  flex-shrink-0
                  justify-center
                  items-center
                  w-12
                  h-12
                  text-white
                  bg-gradient-to-br
                  from-pink-500
                  to-violet-500
                  rounded-lg
                  shadow-md shadow-gray-300
                "
              >
                <HomeIcon class="w-5 h-5"/>
              </div>
              <div class="flex-shrink-0 ml-3">
                <span class="text-2xl font-bold leading-none text-gray-900"
                  >$3,600</span
                >
                <h3 class="text-base font-normal text-gray-500">
                  Today's Money
                </h3>
              </div>
              <div
                class="
                  flex flex-1
                  justify-end
                  items-center
                  ml-5
                  w-0
                  text-base
                  font-bold
                  text-green-500
                "
              >
                +16%
                <HomeIcon class="w-5 h-5"/>
              </div>
            </div>
          </div>
          <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4">
            <div class="flex items-center">
              <div
                class="
                  inline-flex
                  flex-shrink-0
                  justify-center
                  items-center
                  w-12
                  h-12
                  text-white
                  bg-gradient-to-br
                  from-pink-500
                  to-violet-500
                  rounded-lg
                  shadow-md shadow-gray-300
                "
              >
                <HomeIcon class="w-5 h-5"/>
              </div>
              <div class="flex-shrink-0 ml-3">
                <span class="text-2xl font-bold leading-none text-gray-900"
                  >2,300</span
                >
                <h3 class="text-base font-normal text-gray-500">
                  Today's Users
                </h3>
              </div>
              <div
                class="
                  flex flex-1
                  justify-end
                  items-center
                  ml-5
                  w-0
                  text-base
                  font-bold
                  text-green-500
                "
              >
                +3%
                <HomeIcon class="w-5 h-5"/>
              </div>
            </div>
          </div>
          <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4">
            <div class="flex items-center">
              <div
                class="
                  inline-flex
                  flex-shrink-0
                  justify-center
                  items-center
                  w-12
                  h-12
                  text-white
                  bg-gradient-to-br
                  from-pink-500
                  to-violet-500
                  rounded-lg
                  shadow-md shadow-gray-300
                "
              >
                <HomeIcon class="w-5 h-5"/>
              </div>
              <div class="flex-shrink-0 ml-3">
                <span class="text-2xl font-bold leading-none text-gray-900"
                  >+3,462</span
                >
                <h3 class="text-base font-normal text-gray-500">New Clients</h3>
              </div>
              <div
                class="
                  flex flex-1
                  justify-end
                  items-center
                  ml-5
                  w-0
                  text-base
                  font-bold
                  text-red-500
                "
              >
                -2%
                <HomeIcon class="w-5 h-5"/>
              </div>
            </div>
          </div>
          <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4">
            <div class="flex items-center">
              <div
                class="
                  inline-flex
                  flex-shrink-0
                  justify-center
                  items-center
                  w-12
                  h-12
                  text-white
                  bg-gradient-to-br
                  from-pink-500
                  to-violet-500
                  rounded-lg
                  shadow-md shadow-gray-300
                "
              >
                <HomeIcon class="w-5 h-5"/>
              </div>
              <div class="flex-shrink-0 ml-3">
                <span class="text-2xl font-bold leading-none text-gray-900"
                  >$83,430</span
                >
                <h3 class="text-base font-normal text-gray-500">Sales</h3>
              </div>
              <div
                class="
                  flex flex-1
                  justify-end
                  items-center
                  ml-5
                  w-0
                  text-base
                  font-bold
                  text-green-500
                "
              >
                +5.34%
                <HomeIcon class="w-5 h-5"/>
              </div>
            </div>
          </div>
        </div>
</template>
<script setup>
import { HomeIcon } from '@heroicons/vue/outline';
</script>