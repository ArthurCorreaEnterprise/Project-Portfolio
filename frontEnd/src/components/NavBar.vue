<template>
    <nav>
        <div>
            <span>ArthurCorrea</span>
        </div>
        <div class="navbar-style">
            <RouterLink to="/" active-class="active">Home</RouterLink>
            <RouterLink to="/projects" active-class="active">Projects</RouterLink>
            <RouterLink to="/skills" active-class="active">Skills</RouterLink>
            <RouterLink to="/about-me" active-class="active">About Me</RouterLink>
            <RouterLink to="/contact" active-class="active">Contact</RouterLink>
        </div>
        <div>
            <button type="button" class="color-gradient-teal-indigo hoverColor-gradient-indigo-fuchsia">login</button>
        </div>
    </nav>
</template>

<script setup>
import { RouterLink } from 'vue-router'
</script>

<style scoped>
nav {
    @apply flex justify-between items-center py-2 px-6;
    @apply bg-white;
}

span {
    @apply font-lobster-regular text-3xl bg-clip-text text-transparent bg-gradient-to-r;
    @apply from-blue-500 to-violet-500;
}

button.color-gradient-teal-indigo {
  @apply  bg-gradient-to-r;
  @apply  text-white from-teal-500 to-indigo-500;
}

button.hoverColor-gradient-indigo-fuchsia {
  @apply bg-gradient-to-r;
  @apply hover:from-indigo-500 hover:to-fuchsia-500;
}

.navbar-style {
    @apply flex gap-4 font-semibold capitalize text-base;
    @apply text-gray-400;
}

.active {
    @apply text-gray-800 underline;
}
</style>
