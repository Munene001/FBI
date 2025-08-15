<template>
    <section :class="['py-[40px] font-[uno]', light ? 'bg-white' : 'bg-[#FAFAFA]'] ">
      <div class="container mx-auto px-[20px]">
        <SectionHeader :title="title" :subtitle="subtitle" />
        <slot></slot>
      </div>
    </section>
  </template>
  
  <script setup>
  defineProps({
    title: String,
    subtitle: String,
    light: Boolean
  })
  </script>