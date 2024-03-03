<template>
  <div class=" items-center text-center">
    <h2 class="q-ma-none q-mb-md text-weight-bold">{{ title }}</h2>
    <p class="text-subtitle1">{{ desc }}</p>
  </div>
</template>

<script setup lang="ts">
// import { ref } from 'vue'

defineProps({
  title: {
    type: String,
    default: 'Hero Title Placeholder'
  },
  desc: {
    type: String,
    default: 'Hero Description Placeholder'
  }
})
</script>
