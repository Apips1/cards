<script setup lang="ts">
import { ref } from 'vue'
const id = 'ini-id'
const value = 10
const className = 'red bold'
const classNames = ref<string[]>([])
classNames.value.push('red')
classNames.value.push('bold')
</script>

<template>
  <div v-bind:id="id">id</div>
  <div :class="className">red</div>
  <div :class="id == 'ini-id' ? 'bold' : 'red'">red bold</div>
  <div :class="10 < value ? 'red' : 'bold'">kurang dari 10</div>
</template>

<style scoped>
.red {
  color: red;
}
.bold {
  font-weight: bold;
}
</style>
