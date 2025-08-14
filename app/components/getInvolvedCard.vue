<!-- components/GetInvolvedCard.vue -->
<template>
    <div class="bg-white p-[30px] rounded-xl shadow-md text-center" :class="borderRed ? 'border-t-4 border-[#BC361D]' : 'border-t-4 border-[#202654]'">
      <div :class="iconRed ? 'text-[#BC361D] text-[62px]' : 'text-[#202654] text-[62px]'">
        <Icon :name="icon" />
      </div>
      <h3 class="font-bold text-[20px] mb-[15px] text-[#202654]">{{ title }}</h3>
      <slot></slot>
      <button :class="['mt-[20px] px-[20px] py-[10px] rounded-md font-medium', outline ? 'border border-[#202654] text-[#202654]' : 'bg-[#BC361D] text-white']">
        {{ buttonText }}
      </button>
    </div>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    icon: String,
    buttonText: String,
    borderRed: Boolean,
    iconRed: Boolean,
    outline: Boolean
  })
  </script>