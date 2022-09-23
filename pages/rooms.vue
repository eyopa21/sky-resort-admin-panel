<template>
  <div>

    <main>
      <div
        class="block justify-between items-center p-4 mx-4 mt-4 mb-6 bg-white rounded-2xl shadow-xl shadow-gray-200 lg:p-5 sm:flex">
        <div class="mb-1 w-full">
          <div class="mb-4">

            <h1 class="text-xl font-semibold text-gray-900 sm:text-2xl">All Rooms</h1>
          </div>
          <div class="sm:flex">
            <div class="hidden items-center mb-3 sm:flex sm:divide-x sm:divide-gray-100 sm:mb-0">
              <form class="lg:pr-3">
                <label for="users-search" class="sr-only">Search</label>
                <div class="relative mt-1 lg:w-64 xl:w-96">
                  <input type="text" name="email" id="users-search"
                    class="border border-gray-300 text-gray-900 sm:text-sm rounded-lg focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300 block w-full p-2.5"
                    placeholder="Search for users">

                </div>
              </form>
              <div class="flex pl-0 mt-3 space-x-1 sm:pl-2 sm:mt-0">
                <a href="#"
                  class="inline-flex justify-center p-1 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">

                  <CogIcon class="w-6 h-6" />
                </a>
                <a href="#"
                  class="inline-flex justify-center p-1 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
                  <CogIcon class="w-6 h-6" />
                </a>
                <a href="#"
                  class="inline-flex justify-center p-1 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
                  <CogIcon class="w-6 h-6" />
                </a>
                <a href="#"
                  class="inline-flex justify-center p-1 text-gray-500 rounded cursor-pointer hover:text-gray-900 hover:bg-gray-100">
                  <CogIcon class="w-6 h-6" />
                </a>
              </div>
            </div>
            <div class="flex items-center ml-auto space-x-2 sm:space-x-3">
              <button type="button" data-modal-toggle="add-user-modal"
                class="inline-flex items-center py-2 px-3 text-sm font-medium text-center text-white rounded-lg bg-gradient-to-br from-pink-500 to-voilet-500 sm:ml-auto shadow-md shadow-gray-300 hover:scale-[1.02] transition-transform">

                <PlusIcon class="mr-2 -ml-1 w-6 h-6" />
                Add user
              </button>

            </div>
          </div>
        </div>
      </div>
      <div class="flex flex-col my-6 mx-4 rounded-2xl shadow-xl shadow-gray-200">
        <div class="overflow-x-auto rounded-2xl">
          <div class="inline-block min-w-full align-middle">
            <div class="overflow-hidden shadow-lg">
              <table class="min-w-full divide-y divide-gray-200 table-fixed">
                <thead class="bg-white">
                  <tr>
                    <th scope="col" class="p-4 lg:p-5">
                      <div class="flex items-center">
                        <input id="checkbox-all" aria-describedby="checkbox-1" type="checkbox"
                          class="w-5 h-5 rounded border-gray-300 focus:ring-0 checked:bg-dark-900">
                        <label for="checkbox-all" class="sr-only">checkbox</label>
                      </div>
                    </th>
                    <th class="p-4 text-xs font-medium text-left text-gray-500 uppercase lg:p-5">
                      Name
                    </th>
                    <th class="p-4 text-xs font-medium text-left text-gray-500 uppercase lg:p-5">
                      Category
                    </th>
                    <th class="p-4 text-xs font-medium text-left text-gray-500 uppercase lg:p-5">
                      Bed type
                    </th>
                    <th class="p-4 text-xs font-medium text-left text-gray-500 uppercase lg:p-5">
                      Size
                    </th>
                    <th class="p-4 lg:p-5 ">

                    </th>
                  </tr>
                </thead>
                <tbody v-for="i in 5" :key="i" class="bg-white divide-y divide-gray-200">
                  <tr class="hover:bg-gray-100">
                    <td class="p-4 w-4 lg:p-5 ">
                      <div class="flex items-center">
                        <input id="checkbox-1" type="checkbox"
                          class="w-5 h-5 rounded border-gray-300 focus:ring-0 checked:bg-dark-900">
                        <label for="checkbox-1" class="sr-only">checkbox</label>
                      </div>
                    </td>
                    <td class="flex items-center p-4 mr-12 space-x-6 whitespace-nowrap lg:p-5 lg:mr-0">
                      <img class="w-8 h-8 rounded" src="/img/1.png" alt="room image">
                      <div class="text-sm font-normal text-gray-500">
                        <div class="text-base font-semibold text-gray-900">Deluxe room</div>

                      </div>
                    </td>
                    <td class="p-4 text-base font-medium text-gray-900 whitespace-nowrap lg:p-5">Double bed
                    </td>
                    <td class="p-4 text-base font-medium text-gray-900 whitespace-nowrap lg:p-5">Queen bed</td>
                    <td class="p-4 text-base font-normal text-gray-900 whitespace-nowrap lg:p-5">
                      30m<sup>2</sup>
                    </td>
                    <td class="p-4 space-x-2 whitespace-nowrap lg:p-5">
                      <button type="button" data-modal-toggle="user-modal"
                        class="inline-flex items-center py-2 px-3 text-sm font-medium text-center text-gray-700 bg-gray-200 rounded-lg hover:bg-gray-300 hover:text-gray-900 hover:scale-[1.02] transition-all">

                        <PencilAltIcon class="mr-2 w-5 h-5" />
                        Edit user
                      </button>
                      <button type="button" data-modal-toggle="delete-user-modal"
                        class="inline-flex items-center py-2 px-3 text-sm font-medium text-center text-white bg-gradient-to-br from-red-400 to-red-600 rounded-lg shadow-md shadow-gray-300 hover:scale-[1.02] transition-transform">
                        <TrashIcon class="mr-2 w-5 h-5" />
                        Delete user
                      </button>
                    </td>
                  </tr>

                </tbody>
              </table>
            </div>
          </div>
        </div>
      </div>
      <VuePagination />

      

    
     
    </main>
  </div>
</template>
<script setup>
  import {
    CogIcon,
    PlusIcon,
    TrashIcon,
    PencilAltIcon
  } from "@heroicons/vue/outline";
  definePageMeta({
    middleware: "navigation-guard"
  })
</script>