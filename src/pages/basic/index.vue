<script setup lang="ts">
import TextInterpolation from '@/components/text-interpolation.vue'
import rawHtml from '@/components/raw-html.vue'
import AtributeBinding from '@/components/atribute-binding.vue'
import ExpressionVue from '@/components/expression-vue.vue'
import VShow from '@/components/v-show.vue'
import VIf from '@/components/v-if.vue'
import VFor from '@/components/v-for.vue'
import VModel from '@/components/v-model.vue'
import VSlot from '@/components/v-slot.vue'
import ElRef from '@/components/el-ref.vue'
import userComponent from '@/components/user-component.vue'

const userName = ''
</script>

<template>
  <VSlot>
    <template #header> HI </template>
    <TextInterpolation />
    <raw-html />
    <AtributeBinding />
    <ExpressionVue />
    <VShow />
    <VIf />
    <VFor />
    <VModel />
    <ElRef />

    <div v-pre>{{ userName }} {{ user > 23 }}</div>

    <userComponent />
  </VSlot>
</template>

<style scoped></style>
