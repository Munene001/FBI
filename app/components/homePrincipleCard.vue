<template>
    <div 
      class="p-[30px] rounded-xl hover:shadow-lg transition-all h-full"
      :class="dark ? 'bg-[#202654] text-white' : 'bg-[#FAFAFA] border border-gray-200'"
    >
      <div class="text-[#BC361D] text-[40px] mb-[20px]">
        <Icon :name="icon" />
      </div>
      <h3 class="text-[20px] font-bold mb-[15px]">
        <slot name="title">{{ title }}</slot>
      </h3>
      <div class="text-[15px]" :class="dark ? 'text-white/80' : 'text-gray-600'">
        <slot name="description">{{ description }}</slot>
      </div>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: {
      type: String,
      default: ''
    },
    icon: {
      type: String,
      required: true
    },
    description: {
      type: String,
      default: ''
    },
    dark: {
      type: Boolean,
      default: false
    }
  })
  </script>