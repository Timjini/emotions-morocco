<template>
  <main class="space-y-20">
    <HeroSection />
    <PopularDestinations />
    <DestinationGrid />
    <ExclusiveOffer />
    <NightCampSection />
  </main>
</template>

<script setup>
import HeroSection from '../src/components/home/HeroSection.vue'
import PopularDestinations from '../src/components/home/PopularDestinations.vue'
import DestinationGrid from '../src/components/home/DestinationGrid.vue'
import ExclusiveOffer from '../src/components/home/ExclusiveOffer.vue'
import NightCampSection from '../src/components/home/NightCampSection.vue'
</script>
