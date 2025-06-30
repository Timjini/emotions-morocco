<template>
  <div class="max-w-3xl mx-auto px-4 py-8 bg-white space-y-20">
    <!-- Tour Header -->
    <div class="mb-8">
      <h1 class="text-3xl md:text-4xl font-bold text-blue-900 mb-2">Sahara Desert Expedition</h1>
      <div class="flex items-center gap-4 mb-4">
        <span class="bg-yellow-100 text-yellow-800 px-3 py-1 rounded-full text-sm font-bold">
          3 Days / 2 Nights
        </span>
        <span class="text-xl font-bold text-blue-900">€599 per person</span>
      </div>
      <div class="h-px bg-gray-200 w-full my-4"></div>
    </div>

    <!-- Tour Description -->
    <div class="mb-8">
      <h2 class="text-xl font-semibold text-blue-900 mb-4">Tour Description</h2>
      <p class="text-gray-700 mb-6">
        Experience the magic of Morocco's Sahara Desert with our 3-day luxury camping adventure. 
        Ride camels at sunset, sleep under the stars in premium Berber tents, and enjoy traditional 
        Moroccan cuisine.
      </p>

      <!-- Features List -->
      <ul class="space-y-4">
        <li v-for="(feature, index) in features" :key="index" class="flex items-start">
          <div class="bg-yellow-100 p-1.5 rounded-full mr-3 mt-0.5">
            <span class="text-yellow-500 text-lg">{{ featureIcons[index] }}</span>
          </div>
          <div>
            <h3 class="font-bold text-blue-900">{{ feature.title }}</h3>
            <p class="text-gray-600">{{ feature.description }}</p>
          </div>
        </li>
      </ul>
    </div>

    <!-- Booking CTA -->
    <button class="w-full md:w-auto bg-yellow-400 hover:bg-yellow-300 text-blue-900 font-bold py-3 px-8 rounded-lg transition">
      Book Now
    </button>
  </div>
</template>

<script setup>
const features = [
  { title: "Desert Camping", description: "Luxury tents with private facilities" },
  { title: "Camel Trek", description: "Sunset ride through the dunes" },
  { title: "Gourmet Meals", description: "Traditional Moroccan cuisine" },
  { title: "Stargazing", description: "Guided night sky observation" }
]

const featureIcons = ["🏕️", "🐫", "🍽️", "🔭"]
</script>