<template>
    

<div class="hidden md:flex font-[Uno] bg-[#212121]  h-[48px]  text-white justify-between px-5 py-3 font-medium">
  <div class="flex">
    <!-- Time Section -->
    <div class="flex items-center">
      <Icon name="svg-spinners:clock" width="19" height="19" color="white" />
      <p class="ml-2.5">Available 8:00 - 17:00</p>
    </div>
    
    <!-- Phone Numbers -->
    <div class="flex items-center ml-5">
      <Icon name="ic:baseline-phone" width="17" height="17" color="white" />
      <p class="ml-1.5 flex gap-3">
        <span>+254714191919</span>
       
      </p>
    </div>
  </div>
  
  <!-- Email and Social Links -->
  <div class="flex">
    <!-- Email -->
    <div class="flex items-center border-r border-blue-500 pr-6">
      <Icon name="icon-park-outline:mail-download" width="19" height="19" color="white" />
      <p class="ml-2.5 mr-6">draintheswamp@fbikenya.org</p>
    </div>
    
    <!-- Social Icons -->
    <div class="flex items-center gap-3.5 ml-6">
      <a href="https://www.facebook.com" target="_blank" rel="noopener noreferrer" class="hover:opacity-80">
        <Icon name="logos:facebook" width="18" height="18" color="white" />
      </a>
      <a href="https://www.twitter.com" target="_blank" rel="noopener noreferrer" class="hover:opacity-80">
        <Icon name="prime:twitter" width="19" height="19" color="white" />
      </a>
      <a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="hover:opacity-80">
        <Icon name="lineicons:instagram" width="20" height="21" color="white" />
      </a>
      <a href="https://www.linkedin.com" target="_blank" rel="noopener noreferrer" class="hover:opacity-80">
        <Icon name="devicon:linkedin" width="21" height="21" color="white" />
      </a>
    </div>
  </div>
</div>
</template>