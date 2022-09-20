<template>
    <div>
                    <form action="#" method="GET" class="hidden lg:block lg:pl-8">
              <label for="topbar-search" class="sr-only">Search</label>
              <div class="relative mt-1 lg:w-80">
                <div
                  class="
                    flex
                    absolute
                    inset-y-0
                    left-0
                    items-center
                    pl-3
                    pointer-events-none
                  "
                >
                 <SearchIcon class="w-6 h-6"/>
                </div>
                <input
                  type="text"
                  name="email"
                  id="topbar-search"
                  class="
                    bg-gray-50
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
                    block
                    w-full
                    pl-10
                    p-2.5
                  "
                  placeholder="Search"
                />
              </div>
            </form>
    </div>
</template>
<script setup>
import { SearchIcon } from '@heroicons/vue/outline';

</script>