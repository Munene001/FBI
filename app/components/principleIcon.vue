<template>
    <div class="flex flex-col items-center text-center p-[20px]">
      <div class="text-[#BC361D] text-[40px] mb-[15px]">
        <Icon :name="icon" />
      </div>
      <h3 class="font-bold text-[18px] mb-[10px] text-[#202654]">{{ title }}</h3>
      <p class="text-gray-600 text-[14px]">{{ description }}</p>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    icon: String,
    description: String
  })
  </script>