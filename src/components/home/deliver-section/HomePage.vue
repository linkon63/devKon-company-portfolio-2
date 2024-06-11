<template>
  <HeroSections />
  <DeliverSection />

  <OurStrengthsSection />
  <WorkWithUsSection />

  <Testimonials />
  <HireUs />
  <BlogSection />

  <OfficeMaps />
  <AchivementSection />
  <FloatButtons
    class="fixed right-[30px] sm:right-[60px] bottom-[50px] sm:bottom-[100px] z-30"
  />
</template>
<script setup>
import DeliverSection from "../components/home/deliver-section/DeliverSection.vue";
import OurStrengthsSection from "../components/home/our-strengths/OurStrengthsSection.vue";
import WorkWithUsSection from "../components/home/work-with-us/WorkWithUsSection.vue";
import Testimonials from "../components/home/testimonials/Testimonials.vue";
import HireUs from "../components/home/hire-us/HireUs.vue";
import BlogSection from "../components/home/blog-section/BlogSection.vue";
import AchivementSection from "../components/home/achivment-section/AchivementSection.vue";
import OfficeMaps from "../components/home/office-map-section/OfficeMap.vue";
import HeroSection from "../components/home/hero-section/HeroSection.vue";
import HeroSections from "../components/home/hero-section/HeroSections.vue";
import FloatButtons from "../components/buttons/FloatButtons.vue";
//../../components/buttons/ButtonGroup.vue
</script>
