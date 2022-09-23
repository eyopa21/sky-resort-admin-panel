<template>
  <div>
    <nav class="fixed z-30 w-full bg-gray-50">
      <div class="py-3 px-3 lg:px-5 lg:pl-3">
        <div class="flex justify-between items-center">
          <div class="flex justify-start items-center">
            <button
              @click="layout.showSideBar = !layout.showSideBar"
              class="
              block 
              lg:hidden
                p-2
                md:mr-4
                text-gray-600
                rounded
                cursor-pointer
                hover:text-gray-900 hover:bg-gray-100
              "
            >
              <MenuIcon class="h-6 w-6" />
            </button>

            <a
              class="
                hidden
                text-md
                font-semibold
                md:flex
                items-center
                lg:mr-1.5
              "
            >
              <img
                src="/img/1.png"
                class="mr-2 h-8"
                alt="Creative Tim Logo"
              />
              <span
                class="
                  hidden
                  md:inline-block
                  self-center
                  text-xl
                  font-bold
                  whitespace-nowrap
                "
                >Sky resort admin panel</span
              >
            </a>
            <VueSearch />
          </div>
          <div class="relative flex items-center">
            <div>
              <button
                @click="showNotif = !showNotif"
                type="button"
                class="
                  p-2
                  text-gray-500
                  rounded-2xl
                  hover:text-gray-900 hover:bg-gray-100
                "
              >
                <BellIcon class="w-6 h-6" />
              </button>
              <div
                v-if="showNotif"
                class="
                  overflow-hidden
                  absolute
                  top-8
                  md:-left-44
                  z-50
                  my-4
                  max-w-sm
                  text-base
                  list-none
                  bg-white
                  rounded
                  divide-y divide-gray-100
                  shadow-lg shadow-gray-300
                "
              >
                <div
                  class="
                    block
                    py-2
                    px-4
                    text-base
                    font-medium
                    text-center text-gray-700
                    bg-gray-50
                  "
                >
                  Notifications
                </div>
                <div class="">
                  <Notif />
                  <Notif />
                  <Notif />
                  <Notif />
                </div>

                <a
                  href="#"
                  class="
                    flex
                    justify-center
                    py-2
                    text-base
                    font-normal
                    text-center text-gray-900
                    bg-gray-50
                    hover:bg-gray-100
                  "
                >
                  <div class="inline-flex items-center">
                    <HomeIcon class="w-6 h-6" />
                    View all
                  </div>
                </a>
              </div>
            </div>
            <div>
              <button
                @click="showSettings = !showSettings"
                type="button"
                class="
                  p-2
                  text-gray-500
                  rounded-2xl
                  hover:text-gray-900 hover:bg-gray-100
                "
              >
                <HomeIcon class="w-6 h-6" />
              </button>
              <div v-if="showSettings">
                <div
                  class="
                    overflow-hidden
                    z-50
                    my-4
                    text-base
                    list-none
                    rounded
                    shadow-lg shadow-gray-300
                    bg-white
                    absolute
                    top-8
                    -left-12
                  "
                >
                  <div
                    class="
                      py-2
                      px-4
                      text-base
                      font-medium
                      text-center text-gray-700
                      bg-gray-50
                    "
                  >
                    Apps
                  </div>

                  <div class="grid grid-cols-3 gap-4 p-4">
                    <NavSquareTab />
                    <NavSquareTab />
                    <NavSquareTab />
                    <NavSquareTab />
                    <NavSquareTab />
                    <NavSquareTab />
                    <NavSquareTab />
                    <NavSquareTab />
                  </div>
                </div>
              </div>
            </div>
            <div class="ml-3">
              <div>
                <button
                  @click="showUserSettings = !showUserSettings"
                  type="button"
                  class="
                    flex
                    text-sm
                    bg-gray-800
                    rounded-full
                    focus:ring-4 focus:ring-gray-300
                  "
                >
                  <img
                    class="w-8 h-8 rounded-full"
                    src="/img/1.png"
                    alt="user photo"
                  />
                </button>
              </div>
              <div
                v-if="showUserSettings"
                class="
                  absolute
                  z-50
                  my-4
                  text-base
                  list-none
                  bg-white
                  rounded
                  divide-y divide-gray-100
                  shadow-lg shadow-gray-300
                "
              >
                <div class="py-3 px-4" role="none">
                  <p class="text-sm" role="none">Neil Sims</p>
                  <p
                    class="text-sm font-medium text-gray-900 truncate"
                    role="none"
                  >
                    <a href="#">[email&#160;protected]</a>
                  </p>
                </div>
                <ul class="py-1" role="none">
                  <li>
                    <a
                      href="#"
                      class="
                        block
                        py-2
                        px-4
                        text-sm text-gray-700
                        hover:bg-gray-100
                      "
                      role="menuitem"
                      >Dashboard</a
                    >
                  </li>
                  <li>
                    <a
                      href="#"
                      class="
                        block
                        py-2
                        px-4
                        text-sm text-gray-700
                        hover:bg-gray-100
                      "
                      role="menuitem"
                      >Settings</a
                    >
                  </li>
                  <li>
                    <a
                      href="#"
                      class="
                        block
                        py-2
                        px-4
                        text-sm text-gray-700
                        hover:bg-gray-100
                      "
                      role="menuitem"
                      >Earnings</a
                    >
                  </li>
                  <li>
                    <a
                      href="#"
                      class="
                        block
                        py-2
                        px-4
                        text-sm text-gray-700
                        hover:bg-gray-100
                      "
                      role="menuitem"
                      >Sign out</a
                    >
                  </li>
                </ul>
              </div>
            </div>
            <div>
              <a
                href="#"
                class="
                  sm:inline-flex
                  ml-2
                  md:ml-5
                  text-white
                  bg-gradient-to-br
                  from-pink-500
                  to-violet-500
                  font-medium
                  rounded-lg
                  text-xs
                  sm:text-sm
                  px-2
                  md:px-5
                  py-2.5
                  text-left
                  inline-flex
                  items-center
                  md:mr-3
                  shadow-md shadow-gray-300
                  hover:scale-[1.02]
                  transition-transform
                "
              >
                <HomeIcon class="md:mr-2 -ml-1 w-5 h-5" />
                Buy now
              </a>
            </div>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>
<script setup>
import { MenuIcon } from "@heroicons/vue/solid";
import { HomeIcon, BellIcon } from "@heroicons/vue/solid";

const layout = useLayout();


const showNotif = ref(false);
const showSettings = ref(false);
const showUserSettings = ref(false);
</script>
