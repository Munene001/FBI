<template>
    <div class="w-full text-center mb-[30px] relative">
      <!-- Decorative elements -->
      <div class="absolute top-1/2 left-0 w-full h-[1px] bg-gray-200 z-0"></div>
      
      <!-- Main title container -->
      <div class="relative inline-block px-[30px] bg-white z-10">
        <!-- Title with shadow effect -->
        <h2 class="text-[36px] md:text-[48px] font-bold text-[#202654] mb-[12px] tracking-tight leading-tight">
          {{ title }}
        </h2>
        
        <!-- Subtitle with improved spacing -->
        <p v-if="subtitle" class="text-[18px] md:text-[20px] text-gray-600 max-w-[700px] mx-auto">
          {{ subtitle }}
        </p>
        
        <!-- Decorative underline -->
        <div class="mt-[20px]">
          <div class="w-[80px] h-[4px] bg-[#BC361D] mx-auto rounded-full"></div>
          <div class="w-[40px] h-[4px] bg-[#BC361D] mx-auto mt-[4px] opacity-60 rounded-full"></div>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    subtitle: String
  })
  </script>