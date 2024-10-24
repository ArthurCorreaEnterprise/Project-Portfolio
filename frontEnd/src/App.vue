<template>
  <div class="app">
    <header>
      <NavBar />
    </header>
    <RouterView />
    <footer class="copyright">
      <p>© {{ currentYear }} Arthur de Paula Correa. All rights reserved.</p>
    </footer>
  </div>
</template>

<script setup>
import { RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue'

const currentYear = new Date().getFullYear();
</script>

<style scoped>
.app {
  @apply flex flex-col font-sarabun h-screen w-screen;
}

.copyright {
  @apply flex justify-center items-center p-2 bottom-0;
  @apply bg-white text-sm text-gray-500;
}
</style>
