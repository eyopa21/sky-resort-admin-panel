<template>
  <div
    class="
      overflow-y-auto 
      overflow-x-hidden
      flex justify-center
      fixed
      right-0
      left-0
      top-32
      z-50
      text-sm
      items-center
      md:inset-0
      sm:h-screen
      md:h-full
      
    "
   
  >
    <div class="relative px-4 w-full max-w-2xl h-full md:h-auto">
      <div class="relative bg-white rounded-2xl shadow-md shadow-gray-400">
        <div class="flex justify-between items-start p-5 rounded-t border-b">
          <h3 class="text-xl font-semibold">Edit user</h3>
          <button
            @click="test()"
            type="button"
            class="
              text-gray-400
              bg-transparent
              hover:bg-gray-200 hover:text-gray-900
              rounded-2xl
              text-sm
              p-1.5
              ml-auto
              inline-flex
              items-center
            "
          >
            close
          </button>
        </div>

        <div class="p-6 space-y-6">
          <form action="#">
            <div class="grid grid-cols-6 gap-6">
              <div class="col-span-6 sm:col-span-3">
                <label
                  for="first-name"
                  class="block mb-2 text-sm font-medium text-gray-900"
                  >First Name</label
                >
                <input
                  type="text"
                  name="first-name"
                  id="first-name"
                  class="
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
                    block
                    w-full
                    p-2.5
                  "
                  placeholder="Bonnie"
                  required
                />
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label
                  for="last-name"
                  class="block mb-2 text-sm font-medium text-gray-900"
                  >Last Name</label
                >
                <input
                  type="text"
                  name="last-name"
                  id="last-name"
                  class="
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
                    block
                    w-full
                    p-2.5
                  "
                  placeholder="Green"
                  required
                />
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label
                  for="email"
                  class="block mb-2 text-sm font-medium text-gray-900"
                  >Email</label
                >
                <input
                  type="email"
                  name="email"
                  id="email"
                  class="
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
                    block
                    w-full
                    p-2.5
                  "
                  placeholder="example@company.com"
                  required
                />
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label
                  for="phone-number"
                  class="block mb-2 text-sm font-medium text-gray-900"
                  >Phone Number</label
                >
                <input
                  type="number"
                  name="phone-number"
                  id="phone-number"
                  class="
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
                    block
                    w-full
                    p-2.5
                  "
                  placeholder="e.g. +(12)3456 789"
                  required
                />
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label
                  for="department"
                  class="block mb-2 text-sm font-medium text-gray-900"
                  >Department</label
                >
                <input
                  type="text"
                  name="department"
                  id="department"
                  class="
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
                    block
                    w-full
                    p-2.5
                  "
                  placeholder="Development"
                  required
                />
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label
                  for="company"
                  class="block mb-2 text-sm font-medium text-gray-900"
                  >Company</label
                >
                <input
                  type="number"
                  name="company"
                  id="company"
                  class="
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
                    block
                    w-full
                    p-2.5
                  "
                  placeholder="123456"
                  required
                />
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label
                  for="current-password"
                  class="block mb-2 text-sm font-medium text-gray-900"
                  >Current Password</label
                >
                <input
                  type="password"
                  name="current-password"
                  id="current-password"
                  class="
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
                    block
                    w-full
                    p-2.5
                  "
                  placeholder="••••••••"
                  required
                />
              </div>
              <div class="col-span-6 sm:col-span-3">
                <label
                  for="new-password"
                  class="block mb-2 text-sm font-medium text-gray-900"
                  >New Password</label
                >
                <input
                  type="password"
                  name="new-password"
                  id="new-password"
                  class="
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-2 focus:ring-fuchsia-50 focus:border-fuchsia-300
                    block
                    w-full
                    p-2.5
                  "
                  placeholder="••••••••"
                  required
                />
              </div>
            </div>
          </form>
        </div>
        <div class="items-center p-6 rounded-b border-t border-gray-200">
          <button
            class="
              text-white
              bg-black
              font-medium
              rounded-lg
              text-sm
              px-5
              py-2.5
              text-center
              shadow-md shadow-gray-300
              hover:scale-[1.02]
              transition-transform
            "
            type="submit"
          >
            Save all
          </button>
        </div>
      </div>
    </div>
  </div>
  <div class=" fixed h-screen w-screen inset-0 z-40 bg-gray-700 opacity-10"></div>
</template>
<script setup>
import { HomeIcon } from "@heroicons/vue/outline";
const layout = useLayout();

const test = () => {
    layout.value.showModal = false
    console.log("test");
}
</script>