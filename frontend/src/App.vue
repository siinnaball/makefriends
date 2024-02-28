<script setup>
import { RouterView } from 'vue-router'
import navigation from '@/components/NAVI/navigation.vue'

import { useCounterStore } from '@/stores/counter.js'
const store = useCounterStore()
</script>

<template>
  <navigation />
  <RouterView />
</template>

<style scoped></style>
