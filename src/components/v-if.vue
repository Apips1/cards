<script setup lang="ts">
type Status = 'ACTIVE' | 'BAN' | 'INACTIVE'
const status: Status = 'ACTIVE'
</script>

<template>
  <div v-if="status === 'ACTIVE'">ACTIVE</div>
  <div v-else-if="status === 'BAN'">BAN</div>
  <div v-else>INACTIVE</div>
</template>

<style scoped></style>
