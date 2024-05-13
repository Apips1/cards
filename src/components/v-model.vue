<script setup lang="ts">
import { ref } from 'vue'

const input = ref('')
let nonReactive = ''

setTimeout(() => {
  input.value = 'Timeout'
  console.log('a')

  nonReactive = 'Timeout'
}, 3000)
</script>

<template>
  NonReactive: {{ nonReactive }}
  <br />
  hasilnya : {{ input }}
  <br />
  <input type="text" name="" id="" v-model="input" />
</template>

<style scoped></style>
