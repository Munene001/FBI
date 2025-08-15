<template>
    <div class="border border-gray-200 rounded-lg p-[30px] hover:shadow-md transition-all">
      <h3 class="text-[22px] font-bold mb-[15px] flex items-center gap-[10px]" :class="redTitle ? 'text-[#BC361D]' : 'text-[#202654]'">
        <Icon :name="icon" class="text-[50px]" />
        {{ title }}
      </h3>
      <slot></slot>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    icon: String,
    redTitle: Boolean
  })
  </script>