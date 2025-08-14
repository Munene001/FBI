<script setup lang="ts">
import { NuxtLink } from '#components';

</script>

<template>
    <div class="w-[55%] hidden md:flex bg-white px-[30px] font-[uno] py-[30px] text-[#0856a4] flex-col gap-[20px] border border-gray-50 rounded-3xl absolute right-[0%] bottom-[5%] shadow-lg shadow-b shadow-spread z-10">
        <div class="text-[23px] font-semibold">Connect With Our Movement</div>
        <div class="md:grid md:grid-cols-2 gap-[20px]">
            <Iso IconName = "vaadin:handshake" title="Allies & Coalition Partners"  description="Explore partnership opportunities with MVMT"/>
            <Iso IconName = "ix:emergency-stop" title="Rapid Response Line"  description="Report urgent issues needing immediate action"/>
            <Iso IconName = "humbleicons:mail" title="General Inquiries"  description="Contact us at info@mvmt.org for questions"/>
            <Iso IconName = "tabler:microphone" title="Join Our Movement" description="Become part of the change we're building" description2 = "See Volunteer Opportunities"/>
        </div>
        <div class="flex flex-col gap-[20px]">
        <div class="text-center text-[23px] font-semibold">
            <div>Before You Reach Out:</div>
            <div>Have You Checked Our Resources?</div>
        </div>
        <div class="flex flex-row justify-between px-[50px]">
            <div class = "space-x-[4px]">
                <span><Icon name = "devicon:facebook" style="font-size:25px;"/></span>
                <span><Icon name = "mdi:instagram" style="font-size:25px;"/></span>
                <span><Icon name = "prime:twitter" style="font-size:25px;"/></span>
                <span><Icon name = "uiw:linkedin" style="font-size:25px;"/></span>
            </div>
            <a href="/resources" class="bg-[#202654] text-white p-[5px] rounded-md">VIEW RESOURCES</a>
        </div>
        </div>
    </div>
</template>