<template>
    <div
    class=" overflow-y-auto overflow-x-hidden fixed right-0 left-0 top-4 z-50 justify-center items-center md:inset-0 h-modal sm:h-full"
    id="add-user-modal">
    <div class="relative px-4 w-full max-w-2xl h-full md:h-auto">

      <div class="relative bg-white rounded-2xl shadow-lg">

        <div class="flex justify-between items-start p-5 rounded-t border-b">
          <h3 class="text-xl font-semibold">
            Add new user
          </h3>
          <button type="button"
            class="text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-2xl text-sm p-1.5 ml-auto inline-flex items-center"
            data-modal-toggle="add-user-modal">
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd"
                d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
                clip-rule="evenodd"></path>
            </svg>
          </button>
        </div>

        <form action="#">
          <div class="p-6 space-y-6">
            <div class="grid grid-cols-6 gap-6">
              <div class="col-span-6 sm:col-span-3">
                <label for="first-name" class="block mb-2 text-sm font-medium text-gray-900">First Name</label>
                <input type="text" name="first-name" id="first-name"
                  class="shadow-lg-sm border border-gray-300 text-gray-900 sm:text-sm rounded-lg focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300 block w-full p-2.5"
                  placeholder="Bonnie" required>
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label for="last-name" class="block mb-2 text-sm font-medium text-gray-900">Last Name</label>
                <input type="text" name="last-name" id="last-name"
                  class="shadow-lg-sm border border-gray-300 text-gray-900 sm:text-sm rounded-lg focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300 block w-full p-2.5"
                  placeholder="Green" required>
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label for="email" class="block mb-2 text-sm font-medium text-gray-900">Email</label>
                <input type="email" name="email" id="email"
                  class="shadow-lg-sm border border-gray-300 text-gray-900 sm:text-sm rounded-lg focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300 block w-full p-2.5"
                  placeholder="example@company.com" required>
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label for="phone-number" class="block mb-2 text-sm font-medium text-gray-900">Phone Number</label>
                <input type="number" name="phone-number" id="phone-number"
                  class="shadow-lg-sm border border-gray-300 text-gray-900 sm:text-sm rounded-lg focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300 block w-full p-2.5"
                  placeholder="e.g. +(12)3456 789" required>
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label for="department" class="block mb-2 text-sm font-medium text-gray-900">Department</label>
                <input type="text" name="department" id="department"
                  class="shadow-lg-sm border border-gray-300 text-gray-900 sm:text-sm rounded-lg focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300 block w-full p-2.5"
                  placeholder="Development" required>
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label for="company" class="block mb-2 text-sm font-medium text-gray-900">Company</label>
                <input type="number" name="company" id="company"
                  class="shadow-lg-sm border border-gray-300 text-gray-900 sm:text-sm rounded-lg focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300 block w-full p-2.5"
                  placeholder="123456" required>
              </div>
            </div>
          </div>

          <div class="items-center p-6 rounded-b border-t border-gray-200">
            <button
              class="text-white rounded-lg bg-gradient-to-br from-pink-500 to-voilet-500 shadow-md shadow-gray-300 hover:scale-[1.02] transition-transform font-medium text-sm px-5 py-2.5 text-center"
              type="submit">Add user</button>
          </div>
        </form>
      </div>
    </div>
  </div>

</template>