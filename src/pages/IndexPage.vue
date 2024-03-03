<template>
  <q-page class="q-py-lg items-center">

    <IndexHero />

    <q-separator color="primary" />
    <div class="q-px-xl">
      <TechStack />
    </div>
  </q-page>
</template>

<script setup lang="ts">
import IndexHero from 'src/components/IndexHero.vue';
import TechStack from 'src/components/TechStack.vue';
</script>
