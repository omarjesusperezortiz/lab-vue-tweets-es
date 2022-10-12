<template>
   <span class="user">
  <span class="name"> {{userData.name}}</span>
  <span class="handle">{{userData.handle}}</span>
</span>
</template>
<script setup>
//import ref from "vue"

const props = defineProps(['userData'])


</script>
<style scoped>
</style>