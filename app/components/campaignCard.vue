<template>
    <div class="border border-gray-200 rounded-lg p-[30px] hover:shadow-lg transition-all bg-white">
      <div class="flex items-start gap-[20px]">
        <div class="text-[#BC361D] text-[50px]">
          <Icon :name="icon" />
        </div>
        <div>
          <h3 class="text-[22px] font-bold mb-[15px] text-[#202654]">{{ title }}</h3>
          <p class="text-gray-700">{{ description }}</p>
          <ul class="list-disc pl-[20px] mt-[15px] space-y-[10px] text-gray-700">
            <li v-for="(item, index) in items" :key="index">{{ item }}</li>
          </ul>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    icon: String,
    description: String,
    items: Array
  })
  </script>