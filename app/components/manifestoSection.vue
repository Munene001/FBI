<template>
    <div class="w-full text-center mb-[40px] relative">
      <div class="text-[#202654] font-bold text-[28px] md:text-[36px] relative z-10 inline-block px-[20px]">
        <span class="bg-[#FAFAFA] px-[15px]">{{ title }}</span>
      </div>
      <div class="absolute top-1/2 left-0 w-full h-[2px] bg-gradient-to-r from-transparent via-[#BC361D] to-transparent z-0"></div>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String
  })
  </script>