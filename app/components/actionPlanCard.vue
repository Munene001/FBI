<template>
    <div class="border-l-4 border-[#BC361D] pl-[25px] py-[15px]">
      <h3 class="text-[20px] font-bold mb-[15px] text-[#202654]">{{ number }}. {{ title }}</h3>
      <ul class="list-disc pl-[20px] space-y-[10px] text-gray-700">
        <li v-for="(action, index) in actions" :key="index">{{ action }}</li>
      </ul>
    </div>
  </template>
  
  <script setup>
  defineProps({
    number: String,
    title: String,
    actions: Array
  })
  </script>