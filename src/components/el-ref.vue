<template>
  <div ref="div"></div>
</template>

<script setup lang="ts">
import { onMounted, ref } from 'vue'

const div = ref<HTMLElement>()
onMounted(() => {
  console.log(div.value)
})
</script>

<style scoped></style>
