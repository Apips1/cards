<script setup lang="ts">
const rawHtml = '<span style="color: red">Raw HTML</span>'
</script>

<template>
  <div>
    <div v-html="rawHtml"></div>
  </div>
</template>

<style scoped></style>
