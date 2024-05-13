<template>
  <div class="flex justify-center items-center h-screen">
    <div class="relative">
      <div
        class="w-80 h-48 bg-gradient-to-r from-[#9C2CF3] to-[#3A49F9] rounded-3xl relative overflow-hidden"
      >
        <div class="text-white text-sm absolute top-0 left-0 ml-6 mt-6">
          <div>Current Balance</div>
          <div class="text-3xl">$ {{ balance }}</div>
        </div>
        <div class="absolute top-20 right-32 -ml-6 mt-6">
          <div
            class="w-80 h-44 bg-slate-950 opacity-10 border-0"
            style="border-radius: 50% / 50%"
          ></div>
        </div>
        <div class="absolute bottom-24 left-32 -ml-6 mt-6">
          <div
            class="w-80 h-44 bg-slate-950 opacity-10 border-0"
            style="border-radius: 50% / 50%"
          ></div>
        </div>
        <img src="@/assets/img/mastercard.svg" alt="" class="absolute top-0 right-0 mr-6 mt-6" />
        <div class="text-white text-sm absolute bottom-0 left-0 ml-8 mb-8">{{ number }}</div>
        <div class="text-white text-sm absolute bottom-0 right-0 mr-8 mb-8">{{ valid }}</div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  balance?: string
  number?: string
  valid?: string
}>()
</script>

<style scoped></style>
