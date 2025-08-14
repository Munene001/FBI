<!-- components/MissionVisionCard.vue -->
<template>
    <div :class="['p-[30px] rounded-lg', dark ? 'bg-[#202654] text-white' : 'bg-white border border-gray-200']">
      <h3 class="text-[24px] font-bold mb-[15px] flex items-center gap-[10px]">
        <Icon :name="icon" :class="dark ? 'text-[#BC361D] text-[43px]' : 'text-[#202654] text-[43px]'" />
        {{ title }}
      </h3>
      <slot></slot>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    icon: String,
    dark: Boolean
  })
  </script>