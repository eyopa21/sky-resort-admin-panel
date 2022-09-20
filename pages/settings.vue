<template>
   <div>

      <main>
         <div class="grid grid-cols-1 px-4 pt-6 lg:grid-cols-3 lg:gap-6">
            <div class="col-span-full mb-4 lg:mb-0">

               <h1 class="text-xl font-semibold text-gray-900 sm:text-2xl">
                  User settings
               </h1>
            </div>

            <div class="col-span-full lg:col-auto">
               <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4 mb-6">
                  <div class="items-center sm:flex xl:block 2xl:flex sm:space-x-4 xl:space-x-0 2xl:space-x-4">
                     <img class="mb-4 w-28 h-28 rounded-lg sm:mb-0 xl:mb-4 2xl:mb-0 shadow-lg shadow-gray-300"
                        src="../assets/img/1.png" alt="sky logo" />
                     <div>
                        <h3 class="mb-1 text-2xl font-bold text-gray-900">
                           Sky Resorts
                        </h3>
                        <div class="mb-4 text-base font-normal text-gray-500">
                           BahirDar/Ethiopia
                        </div>
                        <a href="#"
                           class="inline-flex items-center py-2 px-3 text-sm font-medium text-center text-white bg-gradient-to-br from-pink-500 to-violet-500 rounded-lg shadow-md shadow-gray-300 hover:scale-[1.02] transition-transform">

                           <ArrowUpIcon class="mr-2 -ml-1 w-4 h-4" />
                           Change Logo
                        </a>
                     </div>
                  </div>
               </div>
              
               <div class="bg-white flex shadow-lg shadow-gray-200 rounded-2xl p-4 mb-6">
                  <div class="items-center sm:flex xl:block 2xl:flex sm:space-x-4 xl:space-x-0 2xl:space-x-4">
                     <img class="mb-4 w-28 h-28 rounded-lg sm:mb-0 xl:mb-4 2xl:mb-0 shadow-lg shadow-gray-300"
                        src="../assets/img/1.png" alt="sky logo" />
                     <div>
                        <h3 class="mb-1 text-2xl font-bold text-gray-900">
                          Backgound image
                        </h3>
                        <div class="mb-4 text-base font-normal text-gray-500">
                           BahirDar/Ethiopia
                        </div>
                        <a href="#"
                           class="inline-flex items-center py-2 px-3 text-sm font-medium text-center text-white bg-gradient-to-br from-pink-500 to-violet-500 rounded-lg shadow-md shadow-gray-300 hover:scale-[1.02] transition-transform">

                           <ArrowUpIcon class="mr-2 -ml-1 w-4 h-4" />
                         Update
                        </a>
                     </div>
                  </div>
               </div>
               


               <SettingsInvitedUsers />
               <SettingsSocialLink />
            </div>
            
            <div class="col-span-2">
               <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4 mb-6">
                  <h3 class="mb-4 text-xl font-bold">General information</h3>
                  <form @submit.prevent="updateInfo()">
                     <div class="grid grid-cols-6 gap-6">
                        <div class="col-span-6 sm:col-span-3">

                           <VueInput label="Hotel Name" type="text" name="Hotel-Name" placeholder="Hotel Name here ..."
                              rule="required" />
                        </div>
                        
                        <div class="col-span-6 sm:col-span-3">

                           <VueInput label="Country" type="text" name="Country" placeholder="Country here ..."
                              rule="required" />
                        </div>
                        <div class="col-span-6 sm:col-span-3">

                           <VueInput label="City" type="text" name="City" placeholder="City here ..." rule="required" />
                        </div>
                        <div class="col-span-6 sm:col-span-3">

                           <VueInput label="Address" type="text" name="Address" placeholder="Address here ..."
                              rule="required" />
                        </div>
                        <div class="col-span-6 sm:col-span-3">

                           <VueInput label="Email" type="email" name="Email" placeholder="Email here ..."
                              rule="email" />
                        </div>
                        <div class="col-span-6 sm:col-span-3">

                           <VueInput label="Phone Number" type="phone" name="Tel-Number"
                              placeholder="Telephone number here ..." rule="required" />
                        </div>

                        <div class="col-span-6 sm:col-full">

                           <VueButton type="submit" name="Save all" />
                        </div>
                     </div>
                  </form>
               </div>
               <SettingsPasswordInfo />
               

            </div>
         </div>

      </main>

   </div>
</template>

<script setup>
import {
   ref
} from "vue";
import {
   ArrowUpIcon
} from "@heroicons/vue/solid";
import {
   useForm
} from "vee-validate";
const {
   handleSubmit
} = useForm();
const updateInfo = handleSubmit((formValues) => {
   console.log(formValues);
});
</script>