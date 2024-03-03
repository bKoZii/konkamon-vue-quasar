<template>
  <q-layout view="hHh LpR fFf" class="body--dark">
    <q-header class="bg-primary text-white" height-hint="98">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="toggleLeftDrawer" />
        <MyName class="q-ml-md" />
      </q-toolbar>
      <q-space />
    </q-header>

    <q-drawer show-if-above bordered v-model="leftDrawerOpen" side="left" :mini="miniState"
      @mouseover="miniState = false" @mouseout="miniState = true" :width=230>
      <q-item to="/" active-class="text-accent" exact v-ripple>
        <q-item-section avatar>
          <q-icon name="home" />
        </q-item-section>
        <q-item-section>
          <q-item-label>Home</q-item-label>
        </q-item-section>
      </q-item>
      <q-item to="/test" active-class="text-accent" v-ripple>
        <q-item-section avatar>
          <q-icon name="code" />
        </q-item-section>
        <q-item-section>
          <q-item-label>Test Page</q-item-label>
        </q-item-section>
      </q-item>
      <q-item to="/about" active-class="text-accent" v-ripple>
        <q-item-section avatar>
          <q-icon name="person" />
        </q-item-section>
        <q-item-section>
          <q-item-label>About</q-item-label>
        </q-item-section>
      </q-item>
    </q-drawer>
    <q-page-container>
      <transition appear enter-active-class="animated fadeIn" leave-active-class="animated fadeOut">
        <router-view />
      </transition>
    </q-page-container>
  </q-layout>
</template>

<script setup lang="ts">
import MyName from 'src/components/Icons/MyName.vue';
import { ref } from 'vue'

const leftDrawerOpen = ref(false)
const miniState = ref(true)

function toggleLeftDrawer() {
  leftDrawerOpen.value = !leftDrawerOpen.value
}
</script>
