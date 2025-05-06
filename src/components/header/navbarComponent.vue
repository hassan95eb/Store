<template>
   <div class="md:flex md:items-center md:gap-12">
      <HeaderMenu />
      <!--profile-->
      <profileComponent />
      <!--profile-->
      <mobileOffcanvas />
   </div>
</template>

<script setup>
import profileComponent from '../profileComponent.vue'
import HeaderMenu from './HeaderMenu.vue'
import mobileOffcanvas from './mobileOffcanvas.vue'
</script>
