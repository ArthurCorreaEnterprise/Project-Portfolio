<template>
  <div class="app">
    <header>
      <NavBar />
    </header>
    <RouterView />
  </div>
</template>

<script setup>
import { RouterView } from 'vue-router'

import NavBar from './components/NavBar.vue'
</script>

<style scoped>
.app {
  @apply font-sarabun
}
</style>
