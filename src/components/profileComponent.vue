<script setup>
import { ref } from 'vue'
const openStatus = ref(false)
const toggleProfile = () => {
  openStatus.value = !openStatus.value
}
</script>
<template>
  <div class="hidden md:relative md:block">
    <button
      @click="toggleProfile"
      type="button"
      class="overflow-hidden rounded-full border border-gray-300 shadow-inner"
    >
      <span class="sr-only">Toggle dashboard menu</span>

      <img
        src="https://images.unsplash.com/photo-1438761681033-6461ffad8d80?q=80&w=1770&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
        alt=""
        class="size-10 object-cover"
      />
    </button>

    <div
      v-show="openStatus"
      class="absolute end-0 z-10 mt-1 w-56 divide-y divide-gray-800 rounded-md border border-gray-700 bg-gray-900 shadow-lg"
      role="menu"
    >
      <div class="p-2">
        <a
          href="#"
          class="block rounded-lg px-4 py-2 text-sm text-gray-500 hover:bg-gray-50 hover:text-gray-700"
          role="menuitem"
        >
          My profile
        </a>

        <a
          href="#"
          class="block rounded-lg px-4 py-2 text-sm text-gray-500 hover:bg-gray-50 hover:text-gray-700"
          role="menuitem"
        >
          Billing summary
        </a>

        <a
          href="#"
          class="block rounded-lg px-4 py-2 text-sm text-gray-500 hover:bg-gray-50 hover:text-gray-700"
          role="menuitem"
        >
          Team settings
        </a>
      </div>

      <div class="p-2">
        <form method="POST" action="#">
          <button
            type="submit"
            class="flex w-full items-center gap-2 rounded-lg px-4 py-2 text-sm text-red-700 hover:bg-red-50"
            role="menuitem"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="size-4"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M9 15 3 9m0 0 6-6M3 9h12a6 6 0 0 1 0 12h-3"
              />
            </svg>

            Logout
          </button>
        </form>
      </div>
    </div>
  </div>
</template>
