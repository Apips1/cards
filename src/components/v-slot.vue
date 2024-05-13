<script setup lang="ts"></script>
<template>
  <header>
    <slot name="header"></slot>
  </header>
  <div class="bg-red">
    <slot></slot>
  </div>
  <footer>copyright {{ new Date().getFullYear() }}</footer>
</template>

<style scoped>
.bg-red {
  background: red;
}
</style>
