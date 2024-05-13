<script setup lang="ts">
const message = ' VUE'
</script>

<template>
  <div v-text="message"></div>
  <div>Hello from {{ message }}</div>
</template>

<style scoped></style>
