<template>
  <div class="home-style">
    <PresentationBanner />
    <SummaryAboutMe />
    <MainProjects />
    <TechnicalSkillsList />
    <Highlights />
    <Testimonials />
    <ContactSection />
  </div>
</template>

<script setup>
import PresentationBanner from '../components/PresentationBanner.vue'
import SummaryAboutMe from '../components/SummaryAboutMe.vue'

</script>

<style scoped>
.home-style {
  @apply h-full w-full flex flex-col
}
</style>
