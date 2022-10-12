<template>
      <img :src=[image] class="profile" alt="profile" />
</template>
<script setup>
import { ref } from 'vue'
const props = defineProps(['image'])





</script>
<style scoped>
</style>