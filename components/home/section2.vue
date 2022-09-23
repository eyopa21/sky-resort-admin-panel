<template>
  <div class="grid grid-cols-1 gap-6 mb-6 w-full md:grid-cols-2 xl:grid-cols-3">
    <div
      class="
        bg-white
        shadow-lg shadow-gray-200
        rounded-2xl
        p-4
        bg-gradient-to-r
        from-dark-800
        to-dark-900
        2xl:col-span-2
      "
    >
      <div class="flex justify-between items-center mb-4">
        <div class="flex-shrink-0">
          <span class="text-2xl font-bold leading-none text-white sm:text-3xl"
            >$45,385</span
          >
          <h3 class="text-base font-normal text-gray-400">Sales this week</h3>
        </div>
        <div
          class="
            flex flex-1
            justify-end
            items-center
            text-base
            font-bold
            text-green-500
          "
        >
          12.5%
          <svg
            class="w-5 h-5"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M5.293 7.707a1 1 0 010-1.414l4-4a1 1 0 011.414 0l4 4a1 1 0 01-1.414 1.414L11 5.414V17a1 1 0 11-2 0V5.414L6.707 7.707a1 1 0 01-1.414 0z"
              clip-rule="evenodd"
            ></path>
          </svg>
        </div>
      </div>
      <div>the chart</div>

      <div
        class="
          flex
          justify-between
          items-center
          pt-3
          mt-5
          border-t border-gray-700
          sm:pt-6
        "
      >
        <div class="relative">
          <button
            class="
              inline-flex
              items-center
              p-2
              text-sm
              font-medium
              text-center text-gray-400
              rounded-2xl
              hover:text-red-500
            "
            type="button"
          >
            Last 7 days

            <div @click="showOptions = !showOptions">
              <HomeIcon class="ml-2 w-4 h-4" />
            </div>
          </button>

          <div
            v-if="showOptions"
            class="
              absolute
              bottom-8
              left-0
              z-50
              my-4
              text-base
              list-none
              bg-white
              rounded
              shadow-lg shadow-gray-200
            "
            id="weekly-sales-dropdown"
          >
            <div class="py-3 px-4" role="none">
              <p class="text-sm font-medium text-gray-900 truncate" role="none">
                Sep 16, 2021 - Sep 22, 2021
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
                  >Yesterday</a
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
                  >Today</a
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
                  >Last 7 days</a
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
                  >Last 30 days</a
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
                  >Last 90 days</a
                >
              </li>
            </ul>
            <div class="py-1" role="none">
              <a
                href="#"
                class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100"
                role="menuitem"
                >Custom...</a
              >
            </div>
          </div>
        </div>
        <div class="flex-shrink-0">
          <a
            href="#"
            class="
              inline-flex
              items-center
              p-2
              text-xs
              font-medium
              text-red-500
              uppercase
              rounded-lg
              sm:text-sm
              hover:bg-gray-700
            "
          >
            Sales Report
            <svg
              class="ml-1 w-4 h-4 sm:w-5 sm:h-5"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M9 5l7 7-7 7"
              ></path>
            </svg>
          </a>
        </div>
      </div>
    </div>
    <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4">
      <div class="flex justify-between items-center mb-4">
        <div>
          <h3 class="mb-2 text-xl font-bold text-gray-900">Sales by Country</h3>
          <span class="text-base font-normal text-gray-500"
            >This is a list of latest country</span
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
                      Sales
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
                      Value
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
                      Bounce
                    </th>
                  </tr>
                </thead>
                <tbody v-for="i in 6" :key="i" class="divide-y divide-gray-200">
                  <tr>
                    <td
                      class="
                        flex
                        items-center
                        p-4
                        text-sm
                        font-normal
                        text-gray-900
                        whitespace-nowrap
                      "
                    >
                      us
                      <span
                        class="
                          mx-5
                          ml-3
                          w-32
                          text-base
                          font-medium
                          text-gray-900
                          sm:flex-none
                        "
                        >United States</span
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
                      9600
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
                      $756,600
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
                      29.6%
                    </td>
                  </tr>
                
                </tbody>
              </table>
            </div>
          </div>
        </div>
      </div>

      <div class="flex justify-between items-center pt-3 border-t sm:pt-6">
        <div class="relative">
          <button
            @click="showOptions = !showOptions"
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
            data-dropdown-toggle="transactions-dropdown"
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

          <div
            v-if="showOptions"
            class="
              absolute
              bottom-8
              z-50
              my-4
              text-base
              list-none
              bg-white
              rounded
              divide-y divide-gray-100
              shadow-lg shadow-gray-200
            "
            id="transactions-dropdown"
          >
            <div class="py-3 px-4" role="none">
              <p class="text-sm font-medium text-gray-900 truncate" role="none">
                Sep 16, 2021 - Sep 22, 2021
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
                  >Yesterday</a
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
                  >Today</a
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
                  >Last 7 days</a
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
                  >Last 30 days</a
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
                  >Last 90 days</a
                >
              </li>
            </ul>
            <div class="py-1" role="none">
              <a
                href="#"
                class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100"
                role="menuitem"
                >Custom...</a
              >
            </div>
          </div>
        </div>
        <div class="flex-shrink-0">
          <a
            href="#"
            class="
              inline-flex
              items-center
              p-2
              text-xs
              font-medium
              text-gray-900
              uppercase
              rounded-lg
              sm:text-sm
              hover:bg-gray-100
            "
          >
            Sales Report
            <svg
              class="ml-1 w-4 h-4 sm:w-5 sm:h-5"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M9 5l7 7-7 7"
              ></path>
            </svg>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { HomeIcon } from "@heroicons/vue/outline";
const showOptions = ref(false);
</script>