<script setup>
import { computed } from 'vue';

const answer = computed(() => {
  return 1 + 1
})
</script>

<template>
  <h1>Vue3</h1>
  <p>1 + 1 = {{ answer }}</p>
</template>