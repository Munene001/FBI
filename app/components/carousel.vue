<template>
    <Carousel v-bind="carouselConfig" class="relative font-[uno]">
    <Slide v-for="slide in slides" :key="slide.id">
      <div class="relative w-full h-[100vh]">
        <!-- Background Image -->
        <img
          :src="slide.image"
          :alt="'Home' + slide.id"
          class="object-center object-cover w-full h-full brightness-75"
        />
        
        <!-- Overlay Content -->
        <div class="absolute inset-0 flex items-center">
          <div class="container mx-auto px-6  md:pt-[138px] pt-[80px]">
            <div class="max-w-2xl bg-black/50 p-8 rounded-lg backdrop-blur-sm">
              <!-- FBI Logo/Title -->
              <div class="flex items-center gap-3 mb-4">
                <div class="bg-[#BC361D] text-white font-bold px-3 py-1 text-xl">
                  FBI
                </div>
                <span class="text-white font-medium">KENYA</span>
              </div>
              
              <!-- Movement Tag -->
              <h1 class="text-4xl md:text-6xl font-bold text-white mb-4 leading-tight">
                FIGHTING BRUTALITY & IMPUNITY
              </h1>
              
              <!-- Tagline -->
              <p class="text-lg md:text-xl text-white/90 mb-6">
                Delivering Dignity, Justice, Safety, and Prosperity to Every Kenyan
              </p>
              
              <!-- Welcome Message -->
              <div class="border-l-4 border-[#BC361D] pl-4 mb-8">
                <p class="text-white/80 italic">
                  "Kenya is a nation of resilience, vibrant communities, and immense natural wealth. 
                  Yet systemic brutality, corruption, and impunity threaten our progress."
                </p>
              </div>
              
              <!-- Slide-specific Slogan -->
              <h2 class="text-2xl md:text-3xl font-semibold text-white mb-6">
                {{ slide.slogan }}
              </h2>
              
              <!-- CTA Button -->
              <NuxtLink 
                to="/contact" 
                class="inline-block bg-[#BC361D] hover:bg-[#a52e17] text-white font-bold px-8 py-3 rounded-md transition-colors"
              >
                Join The Movement
              </NuxtLink>
            </div>
          </div>
        </div>
      </div>
    </Slide>

    <!-- Custom Pagination -->
    <template #addons>
      <Pagination class="absolute bottom-8 left-1/2 transform -translate-x-1/2" />
    </template>
  </Carousel>
</template>
<script setup>
// If you are using PurgeCSS, make sure to whitelist the carousel CSS classes
import "vue3-carousel/carousel.css";
import { Carousel, Slide, Pagination, Navigation } from "vue3-carousel";

const carouselConfig = {
  itemsToShow: 1,
  wrapAround: true,
  autoplay: 4000,
};
const slides = [
  {
    id: 1,
    image: "/homer3.webp",
    slogan: "Our Future. Our Voice. Our Movement.",
  },
  {
    id: 2,
    image: "/team.webp",
    slogan: "Power to the People.",
  },
  {
    id: 3,
    image: "/teamer.webp",
    slogan: "Justice. Equality. Solidarity.",
  },
];
</script>