<script setup lang="ts">
import { NuxtLink } from '#components';

</script>

<template>
    <div class="w-[55%] hidden md:flex bg-white px-[30px] font-[uno] py-[30px] text-[#0856a4] flex-col gap-[20px] border border-gray-50 rounded-3xl absolute right-[0%] bottom-[0%] shadow-lg shadow-b shadow-spread z-10">
    
        <Form/>
        
        <div class="flex flex-col gap-[20px]">
        <div class="flex flex-row justify-between px-[50px]">
            <div class = "space-x-[4px]">
                <span><Icon name = "devicon:facebook" style="font-size:25px;"/></span>
                <span><Icon name = "mdi:instagram" style="font-size:25px;"/></span>
                <span><Icon name = "prime:twitter" style="font-size:25px;"/></span>
                <span><Icon name = "uiw:linkedin" style="font-size:25px;"/></span>
            </div>
            <a href="/manifesto" class="bg-[#202654] text-white p-[5px] rounded-md">MANIFESTO</a>
        </div>
        </div>
    </div>
</template>