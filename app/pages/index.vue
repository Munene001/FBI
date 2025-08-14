<template>
  <Carousel v-bind="carouselConfig">
    <Slide v-for="slide in slides" :key="slide.id">
      <div class="relative w-full h-[100vh]">
        <img
          :src="slide.image"
          :alt="'Home' + slide.id"
          class="object-center object-cover w-full h-full"
        />
        <div class="absolute top-1/2 -left-1/2 translate-x-1/2">
          <div>{{ slide.slogan }}</div>
          <NuxtLink to="/contact" class="bg-red-700 text-white p-[10px]">Join Now</NuxtLink>
        </div>
      </div>
    </Slide>

    <template #addons>
      
      <Pagination />
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
  autoplay: 3300,
};
const slides = [
  {
    id: 1,
    image: "/homer3.webp",
    slogan: "Our Future. Our Voice. Our Movement.",
  },
  {
    id: 2,
    image: "/homer2.webp",
    slogan: "Power to the People.",
  },
  {
    id: 3,
    image: "/homer1.webp",
    slogan: "Justice. Equality. Solidarity.",
  },
];
</script>
