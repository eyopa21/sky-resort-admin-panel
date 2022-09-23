<template>
  <div class="grid grid-cols-1 gap-6 mb-6 w-full md:grid-cols-2">
    <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4">
      <div class="flex justify-between items-center mb-4">
        <div>
          <h3 class="mb-2 text-xl font-bold text-gray-900">User Signups</h3>
          <span class="text-base font-normal text-gray-500"
            >This is a list of latest users</span
          >
        </div>
        <div class="flex-shrink-0">
          <a
            href="#"
            class="
              p-2
              text-sm
              font-medium
              text-gray-900
              rounded-lg
              hover:bg-gray-100
            "
            >View all</a
          >
        </div>
      </div>

      <div class="flex flex-col mt-8">
        <div class="overflow-x-auto rounded-2xl">
          <div class="inline-block min-w-full align-middle">
            <div
              class="overflow-hidden shadow-lg shadow-gray-200 sm:rounded-2xl"
            >
              <table class="min-w-full divide-y divide-gray-200">
                <thead>
                  <tr>
                    <th
                      scope="col"
                      class="
                        p-4
                        text-xs
                        font-medium
                        tracking-wider
                        text-left text-gray-500
                        uppercase
                      "
                    >
                      Name
                    </th>
                    <th
                      scope="col"
                      class="
                        p-4
                        text-xs
                        font-medium
                        tracking-wider
                        text-left text-gray-500
                        uppercase
                      "
                    >
                      Email
                    </th>
                    <th
                      scope="col"
                      class="
                        p-4
                        text-xs
                        font-medium
                        tracking-wider
                        text-left text-gray-500
                        uppercase
                      "
                    >
                      Country
                    </th>
                    <th
                      scope="col"
                      class="
                        p-4
                        text-xs
                        font-medium
                        tracking-wider
                        text-left text-gray-500
                        uppercase
                      "
                    >
                      Role
                    </th>
                    <th
                      scope="col"
                      class="
                        p-4
                        text-xs
                        font-medium
                        tracking-wider
                        text-left text-gray-500
                        uppercase
                      "
                    >
                      Status
                    </th>
                    <th
                      scope="col"
                      class="
                        p-4
                        text-xs
                        font-medium
                        tracking-wider
                        text-left text-gray-500
                        uppercase
                      "
                    >
                      Edit
                    </th>
                  </tr>
                </thead>
                <tbody v-for="i in 5" :key="i" class="divide-y divide-gray-200">
               
                  <tr>
                    <td
                      class="
                        p-4
                        text-sm
                        font-normal
                        text-gray-900
                        whitespace-nowrap
                      "
                    >
                      <div class="flex items-center">
                        <img
                          class="mr-2 w-4 h-4 rounded-full"
                          src="../../assets/img/1.png"
                          alt="Neil image"
                        />
                        Neil Sims
                      </div>
                    </td>
                    <td
                      class="
                        p-4
                        text-sm
                        font-normal
                        text-gray-500
                        whitespace-nowrap
                      "
                    >
                      <a
                        href="https://demos.creative-tim.com/cdn-cgi/l/email-protection"
                        >[email&#160;protected]</a
                      >
                    </td>
                    <td
                      class="
                        p-4
                        text-sm
                        font-semibold
                        text-gray-900
                        whitespace-nowrap
                      "
                    >
                      United States
                    </td>
                    <td
                      class="
                        p-4
                        text-sm
                        font-semibold
                        text-gray-900
                        whitespace-nowrap
                      "
                    >
                      Author
                    </td>
                    <td class="p-4 whitespace-nowrap">
                      <span
                        class="
                          text-white
                          bg-gradient-to-br
                          from-green-500
                          to-green-700
                          text-xs
                          font-bold
                          uppercase
                          mr-2
                          px-2.5
                          py-1
                          
                          rounded-md
                        "
                        >Completed</span
                      >
                    </td>
                    <td class="p-4 whitespace-nowrap">
                  
                      <button
                        @click="layout.showModal = true"
                        type="button"
                        class="
                          text-white
                          bg-gray-800
                
                          font-medium
                          rounded-lg
                          text-sm
                          inline-flex
                          items-center
                          px-2.5
                          py-1.5
                          text-center
                          shadow-md shadow-gray-300
                          hover:scale-[1.02]
                          transition-transform
                        "
                      >
                        <HomeIcon class="mr-1 w-4 h-4" />
                        Edit user
                      </button>
                      <VueModal v-if="layout.showModal"/>
                    </td>
                  </tr>
                  
                </tbody>
              </table>
            </div>
          </div>
        </div>
      </div>

      <div class="flex justify-between items-center pt-3 sm:pt-6">
        <div>
          <button
            class="
              inline-flex
              items-center
              p-2
              text-sm
              font-medium
              text-center text-gray-500
              rounded-2xl
              hover:text-gray-900
            "
            type="button"
            
          >
            Last 7 days
            <svg
              class="ml-2 w-4 h-4"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 9l-7 7-7-7"
              ></path>
            </svg>
          </button>

        </div>
        
      </div>
    </div>
    <div
      class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4 mb-4 xl:mb-0"
    >
      <div class="mb-4">
        <h3 class="mb-2 text-xl font-bold text-gray-900">
          Sessions by country
        </h3>
        <span class="text-base font-normal text-gray-500"
          >View website visitors by hovering over the map</span
        >
      </div>
      <div id="map" class="mb-8"> The map</div>

      <div
        class="
          flex
          justify-between
          items-center
          pt-3
          mt-6
          border-t border-gray-200
          sm:pt-6
        "
      >
        <div>
          <button
            class="
              inline-flex
              items-center
              p-2
              text-sm
              font-medium
              text-center text-gray-500
              rounded-2xl
              hover:text-gray-900
            "
            type="button"
            data-dropdown-toggle="dropdown-sessions-by-country"
          >
            Last 7 days
            <svg
              class="ml-2 w-4 h-4"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 9l-7 7-7-7"
              ></path>
            </svg>
          </button>

        </div>
      
      </div>
    </div>
  </div>
</template>
<script setup>
import { HomeIcon } from '@heroicons/vue/outline';
const layout = useLayout();


const showModal = ref(false)
</script>