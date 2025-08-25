<template>
    <div class="bg-[#202654] text-white rounded-xl p-[30px] hover:shadow-lg transition-all h-full">
      <div class="text-[50px] mb-[20px]" :class="redIcon ? 'text-white' : 'text-white'">
        <Icon :name="icon" />
      </div>
      <h3 class="text-[24px] font-bold mb-[15px]">
        <slot name="title">{{ title }}</slot>
      </h3>
      <div class="space-y-[12px] text-white">
        <slot name="content">
          <ul>
            <li v-for="(item, index) in items" :key="index" class="flex items-start gap-[10px]">
              <div class="text-red-700">•</div>
              <div class="text-gray-200">{{ item }}</div>
            </li>
          </ul>
        </slot>
      </div>
      <NuxtLink 
        :to="link" 
        class="mt-[20px] inline-flex items-center text-white font-medium group"
      >
        <slot name="link-text">Learn more</slot>
        <Icon name="ph:arrow-right" class="ml-[5px] group-hover:translate-x-1 transition-transform" />
      </NuxtLink>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    icon: String,
    items: Array,
    link: String,
    redIcon: Boolean
  })
  </script>