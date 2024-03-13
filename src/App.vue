<script setup>
import { ref, computed } from 'vue';

// const answer = computed(() => {
//   return 1 + 1
// })

const message = computed(() => {
  return 'Hello <strong>' + myName.value  + '</strong>さん'
})
const welcomeColor = 'blue'
const myName = ref('')
</script>

<template>
  <h1>Vue3</h1>
  <!-- <p>1 + 1 = {{ answer }}</p> -->
  <p>お名前は？：<input type="text" size="30" v-model="myName"></p>
  <p v-html="message" :style="{ 'background-color': welcomeColor, color: 'white' }"></p>
  <p v-text="message"></p>
</template>