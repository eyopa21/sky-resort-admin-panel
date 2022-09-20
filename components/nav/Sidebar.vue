<template>
  <div class="w-32">
    <aside class="
        flex
        w-auto
        fixed
        top-0
        left-0
        z-20
        flex-col flex-shrink-0
        pt-16
        h-full
        duration-200
        lg:flex
        transition-width
      ">
      <div class="flex w-64 relative flex-col flex-1 pt-0 min-h-0 bg-gray-50">
        <div class="flex overflow-y-auto flex-col flex-1 pt-8 pb-4">
          <div class="flex-1 px-3 bg-gray-50">
            <ul class="pb-2 pt-1">
              <li>
                <form action="#" method="GET" class="lg:hidden">
                  <label for="mobile-search" class="sr-only">Search</label>
                  <div class="relative">
                    <div class="
                        flex
                        absolute
                        inset-y-0
                        left-0
                        items-center
                        pl-3
                        pointer-events-none
                      ">
                      <div class="w-5 h-5 text-gray-500">
                        <SearchIcon class="w-4 h-4" />
                      </div>

                    </div>
                    <input type="text" name="email" id="mobile-search" class="
                        bg-gray-50
                        border border-gray-300
                        text-dark-500 text-sm
                        font-light
                        rounded-lg
                        focus:ring-2
                        focus:ring-fuchsia-50
                        focus:border-fuchsia-300
                        block
                        w-full
                        pl-10
                        p-2.5
                        mb-2
                      " placeholder="Search" />
                  </div>
                </form>
              </li>
              <div @click="layout.showSideBar = false">
                <NavSideBarTabs name="dashboard" to="/" icon="dashboard" />
                <NavSideBarTabs name="login" to="/auth/login" icon="dashboard" />

                <NavSideBarTabs name="Rooms" to="/rooms" icon='book' />
                <NavSideBarTabs name="Contents" to="/Contents" icon='paper' />
                <NavSideBarTabs name="Gallery" to="/Gallery" icon='gallery' />
                <NavSideBarTabs name="settings" to="/Settings" icon='settings' />
              </div>


            </ul>

          </div>
        </div>
        <!-- bootom ssidebar settings -->
        <div class="relative flex justify-center p-4 space-x-4 w-full bg-gray-100">
          <a href="#" class="
              inline-flex
              justify-center
              p-2
              text-gray-500
              rounded
              cursor-pointer
              hover:text-dark-500 hover:bg-gray-200
            ">
            <HomeIcon class="w-6 h-6" />
          </a>

          <a @mouseenter="showTooltip = true" @mouseleave="showTooltip = false" class="
              inline-flex
              justify-center
              p-2
              text-gray-500
              rounded
              cursor-pointer
              hover:text-dark-500 hover:bg-gray-200
            ">
            <HomeIcon class="w-6 h-6" />
          </a>

          <VueTooltip v-if="showTooltip" class="absolute bottom-14 left-12" />

          <button @click="showLang = !showLang" type="button" data-dropdown-toggle="language-dropdown" class="
              inline-flex
              justify-center
              p-2
              text-gray-500
              rounded
              cursor-pointer
              hover:text-dark-500 hover:bg-gray-200
            ">
            lang
          </button>

          <div v-if="showLang" class="relative">
            <NavLang class="absolute bottom-0 left-2" />
          </div>
        </div>
      </div>
    </aside>
  </div>
</template>
<script setup>
import { HomeIcon, SearchIcon } from "@heroicons/vue/outline";
import { ChevronDownIcon } from "@heroicons/vue/solid";

const layout = uselayout();

const showLang = ref(false);
const showTooltip = ref(false);
const show = ref(false);
</script>