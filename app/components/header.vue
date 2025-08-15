<template>
  <div class="fixed z-50 w-full">
    <Headerlite />
    <!-- Desktop Navigation -->
    <div
      class="h-[90px]  px-[20px] flex-row md:flex hidden w-full bg-[rgba(188,54,29,0.85)] fixed shadow-lg shadow-b shadow-spread"
    >
      <div class="flex w-[25%]  items-center justify-start"><img src="/l.jpeg" alt="logo" class="h-[80%]" /></div>
      <div
        class="flex-1 px-[5px] flex items-center justify-around bg-transparent pr-[10px]"
      >
        <NuxtLink
          to="/"
          class="text-[14px] leading-[14px] text-white font-semibold no-underline hover:underline"
        >
          HOME
        </NuxtLink>
        <NuxtLink
          to="/manifesto"
          class="text-[14px] leading-[14px] font-semibold no-underline text-white hover:underline"
        >
          MANIFESTO
        </NuxtLink>

        <NuxtLink
          to="/about"
          class="text-[14px] leading-[14px] font-semibold no-underline text-white hover:underline"
        >
          ABOUT
        </NuxtLink>
       

        <NuxtLink
          to="/blog"
          class="text-[14px] leading-[14px] font-semibold no-underline text-white hover:underline"
        >
          BLOG
        </NuxtLink>
        <NuxtLink
          to="/contact"
          class="text-[14px] leading-[14px] font-semibold no-underline text-white hover:underline"
        >
          CONTACT US
        </NuxtLink>
      </div>
      <div class="flex items-center gap-[20px] justify-center">
        <button
          @click="scrollTo('contact')"
          class="text-[18px] leading-[14px] rounded-sm font-medium no-underline py-[5px] px-[10px] bg-white text-black flex items-center hover:bg-transparent"
        >
          Donate
          <Icon
            name="icon-park:hand-right"
            class="ml-[10px] h-6 w-6 text-black"
          />
        </button>
      </div>
    </div>

    <!-- Mobile Navigation -->
    <div
      class="flex flex-row max-w-[768px] md:hidden h-[80px] shadow-lg shadow-b shadow-spread z-50 justify-between items-center px-4 box-border bg-[rgba(188,54,29,0.85)]  w-full text-white font-[edgaramond]"
    >
      <div class="flex justify-start h-full items-center"><img src="/l.jpeg" alt="logo" class="h-[80%]"></div>
      <button @click="togglePopup">
        <Icon name="material-symbols:menu" class="text-[28px] text-white" />
      </button>
    </div>

    <!-- Mobile Menu -->
    <div
      v-if="isOpen"
      class="fixed top-0 right-0 flex flex-row w-[90%] h-[100vh] z-50 bg-[rgba(188,54,29,0.95)]  text-white px-[40px] pt-[100px]"
    >
      <div class="flex flex-col gap-[3px] w-full">
        <NuxtLink
          to="/"
          class="flex h-[55px] text-[18px] leading-[18px] font-semibold no-underline border-b border-gray-400 items-center justify-start hover:text-[chocolate]"
        >
          HOME
        </NuxtLink>
        <NuxtLink
          to="/manifesto"
          class="flex h-[55px] text-[18px] leading-[18px] font-semibold no-underline border-b border-gray-400 items-center justify-start hover:text-[chocolate]"
        >
          MANIFESTO
        </NuxtLink>

        <NuxtLink
          to="/about"
          class="flex h-[55px] text-[18px] leading-[18px] font-semibold no-underline border-b border-gray-400 items-center justify-start hover:text-[chocolate]"
        >
          ABOUT US
        </NuxtLink>
       
        <NuxtLink
          to="/blog"
          class="flex h-[55px] text-[18px] leading-[18px] font-semibold no-underline border-b border-gray-400 items-center justify-start hover:text-[#FFD700]"
        >
          BLOG
        </NuxtLink>

        <NuxtLink
          to="/contact"
          class="flex h-[55px] text-[18px] leading-[18px] font-semibold no-underline border-b border-gray-400 items-center justify-start hover:text-[#FFD700]"
        >
          CONTACT US
        </NuxtLink>
      </div>
      <button @click="togglePopup" class="absolute top-[60px] right-[30px]">
        <Icon name="zondicons:close" class="text-[28px] text-[#FFD700]" />
      </button>
    </div>
  </div>
</template>

<script>
import { NuxtLink } from "#components";
import Headerlite from "./headerlite.vue";

export default {
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    togglePopup() {
      console.log("Toggle called! Current state:", this.isOpen);
      this.isOpen = !this.isOpen;
    },
  },
};
</script>
