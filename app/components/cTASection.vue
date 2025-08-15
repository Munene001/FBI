<template>
    <section class="py-[100px] bg-blue-700 bg-cover bg-center relative font-[uno]">
      <div class="absolute inset-0 bg-[#202654]/90"></div>
      <div class="container mx-auto px-[20px] relative z-10 text-center">
        <h2 class="text-[36px] md:text-[48px] font-bold text-white mb-[20px]">
          {{ title }}
        </h2>
        <p class="text-[18px] text-white/80 max-w-[700px] mx-auto mb-[40px]">
          {{ subtitle }}
        </p>
        <div class="flex flex-wrap justify-center gap-[20px]">
          <slot></slot>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    subtitle: String
  })
  </script>