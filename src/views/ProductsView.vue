<template>
  <div>this is products view s</div>
  <div>{{ products }}</div>
</template>

<script setup>
import axios from 'axios'
import { onMounted, ref } from 'vue'
const products = ref([])
onMounted(() => {
  axios
    .get('http://localhost:3000/products')
    .then((res) => {
      products.value = res.data
      console.log(res)
    })
    .catch((error) => {
      console.error(error)
    })
  console.log('axios run')
})
</script>
