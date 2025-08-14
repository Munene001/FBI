<template>
    <div
      class="bg-[#202654] md:w-[57%] md:h-[850px] text-white font-[uno]  md:pt-[30px] flex flex-col gap-[40px] md:gap-[30px] py-[20px] md:shadow-lg md:shadow-r md:shadow-spread md:rounded-r-xl"
    >
      <div class="flex  px-[13px] flex-col gap-[10px]">
        <div class="text-[23px] md:text-[30px] font-semibold">
          <div>We're Here For The People.</div>
          <div>Connect With The MVMT Team</div>
        </div>
        <div class="text-[14px] md:text-[16px]">
          Whether you're a concerned citizen, potential ally organization, or media representative, 
          our dedicated team is ready to engage. Your voice and participation drive our movement forward.
        </div>
      </div>
      <div class="md:hidden px-[13px]">
      <div class=" bg-origin-content md:hidden flex bg-[url('/k.jpg')] h-[378px] bg-cover bg-center rounded-md relative ">
          <span class="absolute top-[20%] left-[25%]"><Icon name = "iconoir:mail-out-solid"  style="font-size:45px; color:green"/></span>
          <span class="absolute bottom-[38%] left-[19%]"><Icon name = "ant-design:message-filled" style="font-size: 35px; color: blue;" /></span>
          <span class="absolute top-[56%] left-[50%]"><Icon name = "tdesign:call-1-filled" style="font-size:50px; color:orangered; " /></span>
          <span class="absolute top-[35%] right-[40%]"><Icon name = "cib:telegram" style="font-size:35px; color: chocolate;"/></span>
          
          <span class="absolute top-[44%] right-[22%] h-[35px] w-[35px]"><img src="/Pn.webp" alt="pin" class="h-full w-full"/></span>
      </div>
      </div>
      <div class="flex flex-col gap-[30px] px-[13px]">
          <div class="flex flex-col gap-[10px]">
        <div class=" text-[22px] font-semibold text-red-400">
          <div>Need Immediate Assistance?</div>
          <div>Contact our rapid response team</div>
        </div>
  
        <button class="bg-white text-[#202654] py-[5px] w-[40%] md:w-[30%] rounded-lg font-semibold">Emergency Line</button>
        </div>
        <button class="flex flex-row items-center gap-[10px]">
          <span><Icon name="logos:whatsapp-icon" style="font-size: 45px;" /></span
          ><span class="font-[15px] text-start">Message Our<br>Organizers</span>
        </button>
      </div>
      <div class="w-full md:hidden flex bg-white px-[30px] py-[30px] text-[#202654] flex-col gap-[40px] border border-gray-50 rounded-3xl shadow-lg shadow-b shadow-spread z-10">
          <div class="text-[23px] font-semibold">Connect With Our Movement</div>
          <div class="grid grid-cols-1 gap-[40px]">
              <Iso IconName = "vaadin:handshake" title="Allies & Coalition Partners"  description="Explore partnership opportunities with MVMT"/>
              <Iso IconName = "ix:emergency-stop" title="Rapid Response Line"  description="Report urgent issues needing immediate action"/>
              <Iso IconName = "humbleicons:mail" title="General Inquiries"  description="Contact us at info@mvmt.org for questions"/>
              <Iso IconName = "tabler:microphone" title="Join Our Movement" description="Become part of the change we're building" description2 = "See Volunteer Opportunities"/>
          </div>
          <div class="flex flex-col gap-[30px]">
          <div class="text-center text-[23px] font-semibold">
              <div>Before You Reach Out:</div>
              <div>Have You Checked Our Resources?</div>
          </div>
          <div class="flex flex-row justify-between items-center">
              <div class = "space-x-[4px]">
                  <span><Icon name = "devicon:facebook" style="font-size:25px;"/></span>
                  <span><Icon name = "mdi:instagram" style="font-size:25px;"/></span>
                  <span><Icon name = "prime:twitter" style="font-size:25px;"/></span>
                  <span><Icon name = "uiw:linkedin" style="font-size:25px;"/></span>
                  
              </div>
              <a href="/resources" class="bg-[#202654] text-white p-[10px] rounded-md">VIEW RESOURCES</a>
          </div>
          </div>
          
      </div>
  
     
    
      
     
      <div class=" flex flex-col gap-[10px] px-[13px]">
        <div class="text-[21px] font-semibold">Visit Our Headquarters</div>
        <button class="flex flex-row gap-[10px]">
          <span><Icon name="tdesign:location-filled" style="font-size: 50px; color:white" /></span
          ><span class="flex flex-col text-start font-[16px]"
            ><span>People's Movement Center</span> <span>123 Democracy Ave</span
            ><span>View on Google Maps</span></span
          >
        </button>
      </div>
      <div class="font-semibold hidden md:flex gap-[50px] px-[13px]">
          <div>
          <div>FOLLOW OUR MOVEMENT : </div>
          <div>CHECK OUR ORGANIZING RESOURCES</div>
          </div>
          <div>
              <Icon name = "fontisto:arrow-right-l" style="font-size: 40px;"/>
              </div>
      </div>
    </div>
  </template>