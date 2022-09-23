<template>
  <main class="bg-gray-50">
    <div class="flex flex-col justify-center items-center px-6 pt-8 mx-auto md:h-screen pt:mt-0">
      <NuxtLink class="flex justify-center items-center mb-8 text-2xl font-semibold lg:mb-10">
        <img src="../../assets/img/1.png" class="mr-4 h-10" alt="Sky hotel logo" />
        <span class="self-center text-2xl font-bold whitespace-nowrap">SkyResort admin</span>
      </NuxtLink>

      <div class="w-full bg-white rounded-2xl shadow-xl shadow-gray-300 md:mt-0 sm:max-w-screen-sm xl:p-0">
        <div class="p-10 w-full">
          <h2 class="mb-3 text-2xl font-bold text-gray-900 lg:text-3xl">
            Forgot your password?
          </h2>
          <p class="text-base font-normal text-gray-500">
            Don't fret! Just type in your email and we will send you a code to
            reset your password!
          </p>
          <form class="mt-8 space-y-6" @submit.prevent="forgot()">
            <div>
              
                <VueInput name="Email" type="email" placeholder="Please insert the email here..." rule="email" label="Your Email"/>
            </div>
            <div class="flex items-start">
              <div class="flex items-center h-5">
                <input id="remember" aria-describedby="remember" name="remember" type="checkbox"
                  class="w-5 h-5 rounded border-gray-300 focus:ring-3 focus:ring-0 checked:bg-dark-900" required />
              </div>
              <div class="ml-3 text-sm">
                <label required for="remember" class="font-medium text-gray-900">I accept the
                  <div href="#" class="text-fuchsia-500 hover:underline">Terms and Conditions</div>
                </label>
              </div>
            </div>
            <VueButton name="Reset password" type="submit" />
          </form>
        </div>
      </div>
    </div>
  </main>
</template>
<script setup>

import { useForm } from "vee-validate";

const { handleSubmit } = useForm();

const forgot = handleSubmit((formValues) => {
  console.log(formValues);
});

definePageMeta({ middleware: "navigation-guard" })
</script>