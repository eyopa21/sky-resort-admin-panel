<template>
    <li>
                <NuxtLink
                  :to="props.to"
                  class="
                    flex
                    items-center
                    py-2.5
                    px-4
                    text-base
                    font-normal
                    text-dark-500
                    rounded-lg
                    hover:bg-gray-200
                    group
                    transition-all
                    duration-200
                  "
                  sidebar-toggle-collapse
                >
                  <div
                    class="
                      bg-white
                      shadow-lg shadow-gray-300
                      text-dark-700
                      w-8
                      h-8
                      p-2.5
                      mr-1
                      rounded-lg
                      text-center
                      grid
                      place-items-center
                    "
                  >
                   <AdjustmentsIcon class="h-3 w-3" v-if="props.icon=='dashboard'"/>
                   <PhotographIcon class="h-3 w-3" v-if="props.icon=='gallery'"/>
                   <BookOpenIcon class="h-3 w-3" v-if="props.icon=='book'"/>
                   <NewspaperIcon class="h-3 w-3" v-if="props.icon=='paper'"/>
                   <CogIcon class="h-3 w-3" v-if="props.icon=='settings'"/>
                  </div>
                  <span
                    class="ml-3 text-dark-500 text-sm font-light"
                    sidebar-toggle-item
                    >{{props.name}}</span
                  >
                </NuxtLink>
              </li>
</template>
<script setup>
import { HomeIcon, AdjustmentsIcon, CogIcon, NewspaperIcon, BookOpenIcon, PhotographIcon } from '@heroicons/vue/solid';
const props = defineProps({
    name: {
        type: String,
        required: true
    },
    to: {
        type:  String,
        required: true
    },
    icon: {
      type: String,
      required: true
    }
})
</script>