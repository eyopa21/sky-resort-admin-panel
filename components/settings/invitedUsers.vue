<template>
    <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4 mb-6">
        <div class="flow-root">
           <h3 class="text-xl font-bold">Invited Admins</h3>
           <ul class="mb-6 divide-y divide-gray-200">
              <li v-for="i in 4" :key="i" class="py-4">
                 <div class="flex justify-between xl:block 2xl:flex align-center 2xl:space-x-4">
                    <div class="flex space-x-4 xl:mb-4 2xl:mb-0">
                       <div>
                          <img class="w-6 h-6 rounded-full" src="/img/1.png"
                             alt="Bonnie image" />
                       </div>
                       <div class="flex-1 min-w-0">
                          <p class="text-base font-semibold text-gray-900 leading-none truncate mb-0.5">
                             Bonnie Green
                          </p>
                          <p class="mb-1 text-sm font-normal text-fuchsia-600 truncate">
                             New York, USA
                          </p>
                          <p class="text-xs font-medium text-gray-500">
                             Last seen: 1 min ago
                          </p>
                       </div>
                    </div>
                    <div class="inline-flex items-center w-auto lg:w-full 2xl:w-auto space-x-2">
                       <button 
                          class="py-2 px-3 w-1/2 text-sm font-medium text-center text-gray-900 bg-white rounded-lg border border-gray-300 hover:bg-gray-100 focus:ring-4 focus:ring-fuchsia-200">Suspend</button>
                          <button 
                          class="py-2 px-3 w-1/2 text-sm font-medium text-center text-gray-200 bg-gradient-to-br from-red-500 to-pink-500 rounded-lg border border-gray-300 hover:scale-[1.02] focus:ring-4 focus:ring-fuchsia-200">Delete</button>
                    </div>
                 </div>
              </li>
              
           </ul>
           <div>
              <button
                 class="text-white bg-gradient-to-br from-pink-500 to-violet-500 rounded-lg shadow-md shadow-gray-300 hover:scale-[1.02] transition-transform font-medium text-sm px-5 py-2.5 text-center">
                 Save all
              </button>
           </div>
        </div>
     </div>
</template>