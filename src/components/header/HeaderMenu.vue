<template>
  <nav aria-label="Global" class="hidden md:block">
    <ul class="flex items-center gap-6 text-sm">
      <li>
        <RouterLink
          class="text-white transition hover:text-cyan-600"
          to="/"
          active-class="custom-active-menu-link"
        >
          Home
        </RouterLink>
      </li>
      <li>
        <RouterLink class="text-white transition hover:text-cyan-600" to="/products">
          Products
        </RouterLink>
      </li>
    </ul>
  </nav>
</template>
<style scoped>
.router-link-exact-active {
  font-weight: 600;
  color: #009689;
}
</style>
