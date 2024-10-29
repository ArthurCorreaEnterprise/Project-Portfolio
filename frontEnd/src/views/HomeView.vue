<template>
  <div class="home-style">
    <PresentationBanner />
    <!-- <SummaryAboutMe /> -->
     <!-- <AreasOfExpertise /> -->
    <!-- <TechnicalSkillsList /> -->
    <MainProjects />
    <Highlights />
    <Testimonials />
    <ContactSection />
  </div>
</template>

<script setup>
import PresentationBanner from '../components/PresentationBanner.vue'
// import SummaryAboutMe from '../components/SummaryAboutMe.vue'
// import AreasOfExpertise from '../components/AreasOfExpertise.vue'
// import TechnicalSkillsList from '../components/TechnicalSkillsList.vue'

</script>

<style scoped>
.home-style {
  @apply h-full w-full flex flex-col
}
</style>
