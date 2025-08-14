<script setup lang="ts">


</script>

<template>
    <div  class="md:flex md:flex-row relative md:bg-[#0856a4] font-uno md:pt-[138px] pt-[80px]">
    <Cpart/>
    <Part/>
    <div class=" hidden md:flex bg-[url('/k.jpg')] h-[500px] bg-cover bg-center flex-1 relative ">
        <span class="absolute top-[14%] left-[28%]"><Icon name = "iconoir:mail-out-solid"  style="font-size:45px; color:green"/></span>
        <span class="absolute bottom-[38%] left-[29%]"><Icon name = "ant-design:message-filled" style="font-size: 35px; color: blue;" /></span>
        <span class="absolute top-[16%] left-[50%]"><Icon name = "tdesign:call-1-filled" style="font-size:50px; color:orangered; " /></span>
        <span class="absolute top-[87%] right-[35%]"><Icon name = "cib:telegram" style="font-size:35px; color: chocolate;"/></span>
        <span class="absolute top-[44%] right-[34%] h-[35px] w-[35px]"><img src="/Pn.webp" alt="pin" class="h-full w-full"/></span>
    </div>
    </div>
    
    </template>