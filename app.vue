<template>
  <div class="text-5xl">
  
    
    <NuxtLayout name="default" >
      <NuxtPage :class="{'lg:pl-64 pt-16 ': $route.name !== 'auth-login'}"/>
    </NuxtLayout>
  
  </div>
    
  </template>
  
  <script setup>
  
  </script>
  
  