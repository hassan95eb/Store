<template>
   <header class="bg-gray-900 sticky top-0">
      <div class="mx-auto max-w-screen-xl px-4">
         <div class="flex h-16 items-center justify-between">
            <logoComponent />
            <navbarComponent />
         </div>
      </div>
   </header>
</template>

<script setup>
import navbarComponent from './navbarComponent.vue'
import logoComponent from './logoComponent.vue'
</script>
