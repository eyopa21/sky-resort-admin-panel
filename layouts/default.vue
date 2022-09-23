<template>
  <div class="bg-gray-50 min-h-screen">
    <NavNavv v-if="$route.name !== 'auth-login' || $route.name !== 'auth-login' " />
    <div v-if="$route.name !== 'auth-login'"  @click="showSideBar=false"  :class="layout.showSideBar ? 'block' : 'hidden lg:block'"
      class="flex overflow-hidden bg-white">
      <NavSidebar />
      <div class="block lg:hidden fixed inset-0 z-10 bg-gray-900 opacity-50"></div>
    </div>
    <slot />
    <div v-if="$route.name !== 'auth-login'" class="h-full pt-6 bg-gray-50 relative overflow-y-auto lg:ml-64">
      <footer-footerr />
    </div>
  </div>
</template>
<script setup>
const showSideBar = ref(false);
const layout = useLayout();
</script>