<template>
  <div :class="`${bg} pa-6 rounded-lg shadow-md`">
    <slot></slot>
  </div>
</template>

<script setup>
import { defineProps } from 'vue'

defineProps({
  bg: {
    type: String,
    default: 'bg-gray-100',
  },
})
</script>
