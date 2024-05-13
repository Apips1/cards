<template>
  {{ user.createdAt }}
  <button @click="updateDate">Update Date</button>
  <div>Formated Date: {{ formatedDate }}</div>
  <div>{{ user.createdAt.getMilliseconds() }}</div>
  <div>{{ user.createdAt.getMilliseconds() }}</div>
</template>

<script setup lang="ts">
import { ref, computed, watchEffect, watch } from 'vue'

const user = ref({
  name: 'username',
  createdAt: new Date()
})

const formatedDate = computed(() => {
  return user.value.createdAt.getMilliseconds()
})

const updateDate = () => {
  user.value.createdAt = new Date()
}

watchEffect(() => {
  console.log(formatedDate.value)
})
watch(formatedDate, () => {
  console.log('berubah')
})
</script>

<style scoped></style>
