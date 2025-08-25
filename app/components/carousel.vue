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
        <div class="absolute inset-0 flex items-center md:pt-[40px]">
          <div class="container mx-auto px-6 md:px-4">
            <div
              class="max-w-2xl bg-black/20 p-6 md:p-6 rounded-lg backdrop-blur-sm"
            >
              <!-- FBI Logo/Title -->
              <div
                class="flex flex-col md:flex-row items-start md:items-center gap-2 md:gap-2 mb-4 md:mb-2"
              >
                <div
                  class="bg-[#BC361D] text-white font-bold px-3 md:px-2 py-1 text-lg md:text-lg flex items-center"
                >
                  FBI
                  <span class="ml-2 md:ml-1 text-sm md:text-[19px] font-normal"
                    >(Fighting Brutality & Impunity)</span
                  >
                </div>
                <span
                  class="text-white font-medium bg-black/30 px-3 md:px-2 py-1 rounded-md"
                  >KENYA</span
                >
              </div>

              <!-- Movement Tag -->
              <h1
                class="text-3xl md:text-5xl font-bold text-white mb-4 md:mb-2 leading-tight"
              >
                FIGHTING BRUTALITY & IMPUNITY
              </h1>

              <!-- Tagline -->
              <p class="text-[17px] md:text-[19px] text-white/90 mb-3 md:mb-3">
                Delivering Dignity, Justice, Safety, and Prosperity to Every
                Kenyan
              </p>

              <!-- Welcome Message -->
              <div
                class="border-l-4 border-[#BC361D] pl-4 md:pl-3 mb-8 md:mb-4"
              >
                <p class="text-white/80 italic text-sm">
                  "Kenya is a nation of resilience, vibrant communities, and
                  immense natural wealth. Yet systemic brutality, corruption,
                  and impunity threaten our progress."
                </p>
              </div>

              <!-- Integrated CTA Section -->
              <div
                class="mt-2 md:mt-4 pt-4 md:pt-3 border-t border-[#BC361D]/30"
              >
                <div class="flex items-center">
                  <div class="flex-shrink-0 text-[#BC361D] mr-3 md:mr-2">
                    <Icon name="mdi:account-group" class="text-[19px]" />
                  </div>
                  <div>
                    <h3 class="text-lg md:text-[19px] font-semibold text-white">
                      Join 15,000+ Kenyans in the movement
                    </h3>
                    <p class="text-white/80 text-sm md:text-xs">
                      Add your voice below to help build a better Kenya
                    </p>
                  </div>
                </div>
                <div
                  class="mt-3 md:mt-2 flex items-center cta-pulse text-[#BC361D] font-medium"
                >
                  <span>Complete the form to join us</span>
                  <Icon
                    name="mdi:arrow-down"
                    class="text-[25px] text-white ml-2 md:ml-1"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </Slide>

    <!-- Custom Pagination -->
    <template #addons>
      <Pagination
        class="absolute bottom-8 left-1/2 transform -translate-x-1/2"
      />
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
  autoplay: 5000,
};
const slides = [
  {
    id: 1,
    image: "/injustice4.webp",
    slogan: "Our Future. Our Voice. Our Movement.",
  },
  {
    id: 2,
    image: "/injustice3.webp",
    slogan: "Power to the People.",
  },
  {
    id: 3,
    image: "/injustice2.webp",
    slogan: "Justice. Equality. Solidarity.",
  },
];
</script>
