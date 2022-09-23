<template>
  <main class="bg-gray-50 pt-0">
    <div class="
        flex flex-col
        justify-center
        items-center
        px-6
        pt-8
        mx-auto
        md:h-screen
        
      ">
      <div class="
          p-10
          w-full
          max-w-lg
          bg-white
          rounded-2xl
          shadow-xl shadow-gray-300
        ">
        <h2 class="text-2xl font-bold text-gray-900">Sign in to SkyResort Admin Panel</h2>
        <div class="space-y-8">
          <h2 class="text-md  text-gray-900">Control SkyResort hotel here!!</h2>

          <form @submit.prevent="login()" class="mt-8 space-y-6" >
            <VueInput name="Email" label="Email" type="text" placeholder="Email here..." rule="required" />
            <VueInput name="Password" label="Password" type="password" placeholder="Password here..." rule="required" />
            <div class="flex items-start">
              <div class="flex items-center h-5">
                <input id="remember" aria-describedby="remember" name="remember" type="checkbox" class="
                    w-5
                    h-5
                    rounded
                    border-gray-300
                    focus:outline-none focus:ring-0
                    checked:bg-dark-900
                  "  />
              </div>
              <div class="ml-3 text-sm">
                <label for="remember" class="font-medium text-gray-900">Remember me</label>
              </div>
              <NuxtLink to="/auth/forgot" class="ml-auto text-sm text-fuchsia-600 hover:underline">Lost Password?
              </NuxtLink>
            </div>
            <button type="submit" class="
                py-3
                px-5
                w-full
                text-base
                font-medium
                text-center text-white
                bg-gradient-to-br
                from-pink-500
                to-violet-500
                hover:scale-[1.02]
                shadow-md shadow-gray-300
                transition-transform
                rounded-lg
                sm:w-auto
              ">
              Login to your account
            </button>

          </form>
        </div>
      </div>
    </div>
  </main>
</template>

<script setup>
import { DatabaseIcon } from "@heroicons/vue/outline";
import { useForm } from "vee-validate";

const { handleSubmit } = useForm();

const login = handleSubmit((formValues) => {
  console.log(formValues);
});



definePageMeta({ middleware: "navigation-guard" })
</script>