<script setup>
import headerComponent from './components/header/headerComponent.vue'
import footerComponent from './components/footer/footerComponent.vue'
</script>
<template>
   <headerComponent />
   <RouterView />
   <footerComponent />
</template>
