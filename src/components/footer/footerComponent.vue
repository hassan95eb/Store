<script setup>
import footerMenu from './footerMenu.vue'
import contactMeFooter from './contactMeFooter.vue'
</script>

<template>
  <footer class="bg-gray-900 lg:grid lg:grid-cols-5">
    <div class="relative block h-32 lg:col-span-2 lg:h-full">
      <img
        src="https://images.unsplash.com/photo-1642370324100-324b21fab3a9?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1548&q=80"
        alt=""
        class="absolute inset-0 h-full w-full object-cover"
      />
    </div>

    <div class="px-4 py-16 sm:px-6 lg:col-span-3 lg:px-8">
      <div class="grid grid-cols-1 gap-8 sm:grid-cols-2">
        <contactMeFooter />
        <div class="grid grid-cols-1 gap-4 sm:grid-cols-2">
          <div>
            <p class="font-medium text-gray-900 dark:text-white">Services</p>
            <footerMenu />
          </div>
          <div>
            <p class="font-medium text-gray-900 dark:text-white">Company</p>
            <footerMenu />
          </div>
        </div>
      </div>

      <div class="mt-12 border-t border-gray-100 pt-12 dark:border-gray-800">
        <div class="sm:flex sm:items-center sm:justify-between">
          <p class="mt-8 text-xs text-gray-500 sm:mt-0 dark:text-gray-400">
            &copy; 2022. Company Name. All rights reserved.
          </p>
        </div>
      </div>
    </div>
  </footer>
</template>
