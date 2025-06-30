<template>
  <main class="space-y-20">
    <HeroSection />
    <PopularDestinations />
    <ExclusiveOffer />
    <DestinationGrid />
    <ExperienceSection />
  </main>
</template>

<script setup>
import Navbar from '../src/components/common/Navbar.vue'
import HeroSection from '../src/components/home/HeroSection.vue'
import PopularDestinations from '../src/components/home/PopularDestinations.vue'
import DestinationGrid from '../src/components/home/DestinationGrid.vue'
import ExclusiveOffer from '../src/components/home/ExclusiveOffer.vue'
import ExperienceSection from '../src/components/home/ExperienceSection.vue'
import Footer from '../src/components/common/Footer.vue'
</script>
