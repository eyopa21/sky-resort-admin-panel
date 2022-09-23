<template>
<ul  class=" z-50 my-4 text-base list-none bg-white rounded divide-y divide-gray-100 shadow-lg" id="language-dropdown">

<li>
<a href="#" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200" role="menuitem">
<div class="inline-flex items-center">

English (US)
</div>
</a>
</li>
<li>
<a href="#" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200" role="menuitem">
<div class="inline-flex items-center">

Deutsch
</div>
</a>
</li>
<li>
<a href="#" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200" role="menuitem">
<div class="inline-flex items-center">

Italiano
</div>
</a>
</li>
<li>
<a href="#" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-200" role="menuitem">
<div class="inline-flex items-center">

中文 (繁體)
</div>
</a>
</li>
</ul>

</template>
<script setup>
import { HomeIcon } from '@heroicons/vue/outline';
const showLang = ref(false)
</script>