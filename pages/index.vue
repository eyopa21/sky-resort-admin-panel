<template>
  <div class="font-bold text-5xl lg:pl-64">
    <main>
      <div class="px-4 pt-6">
        <!--section 1-->
        <HomeSection1 />
        <!--section 2-->
        <HomeSection2 />
        <!--section 3-->
        <HomeSection3 />
        <!--section 4-->
        <HomeSection4 />

      </div>
    </main>
  </div>
</template>
<script setup>
import { HomeIcon } from "@heroicons/vue/outline";



definePageMeta({middleware: "navigation-guard"})
</script>