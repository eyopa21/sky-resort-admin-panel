<template>
    <div class="bg-white shadow-lg shadow-gray-200 rounded-2xl p-4 mb-6">
        <h3 class="mb-4 text-xl font-bold">Password information</h3>
        <form @submit.prevent="changePass()">
           <div class="grid grid-cols-6 gap-6">
              <div class="col-span-6 sm:col-span-3">
                
                    <VueInput label="Current password" type="text" name="Current-Password" placeholder="Current password here ..."
                    rule="required" />
              </div>
              <div class="col-span-6 sm:col-span-3">
                 
                    <VueInput label="New password" type="password" name="New-password" placeholder="********"
                    rule="password" />
              </div>
              <div class="col-span-6 sm:col-span-3">
                
                    <VueInput label="COnfirm password" type="password" name="Confirm-password" placeholder="*********"
                    rule="confirmed:@New-password" />
              </div>
              <div class="col-span-full">
                 <div class="text-sm font-medium">
                    Password requirements:
                 </div>
                 <div class="mb-1 text-sm font-normal text-gray-500">
                    Ensure that these requirements are met:
                 </div>
                 <ul class="pl-4 space-y-1 text-gray-500">
                    <li class="text-xs font-normal">
                       At least 10 characters (and up to 100 characters)
                    </li>
                    <li class="text-xs font-normal">
                       At least one lowercase character
                    </li>
                    <li class="text-xs font-normal">
                       Inclusion of at least one special character, e.g., ! @
                       # ?
                    </li>
                    <li class="text-xs font-normal">
                       Some text here zoltan
                    </li>
                 </ul>
              </div>
              <div class="col-span-6 sm:col-full">
                 
                 <VueButton name="Change" type="submit"/>
              </div>
           </div>
        </form>
     </div>
</template>

<script setup>

import { DatabaseIcon } from "@heroicons/vue/outline";
import { useForm } from "vee-validate";

const { handleSubmit } = useForm();

const changePass = handleSubmit((formValues) => {
  console.log(formValues);
});


</script>