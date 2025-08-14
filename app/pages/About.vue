<script setup lang="ts">
import { NuxtLink } from "#components";
</script>

<template>
  <div>
    <!-- Hero Section -->
    <div class="bg-[url('/team.webp')] pt-[87px] h-[60vh] md:h-[85vh] bg-cover bg-center md:pt-[145px] px-[10px] font-uno flex flex-col items-center justify-center">
      <NuxtLink
        to="/contact"
        class="border-2 font-semibold border-white text-white p-[7px] hover:bg-white hover:text-[#202654] transition-colors mb-4"
        >Join The Movement</NuxtLink
      >
      <h1 class="text-[38px] md:text-[48px] leading-[1.2] font-bold text-white text-center">
        About FBI Kenya
      </h1>
      <p class="text-white mt-4 max-w-[600px] text-center px-4">
        Fighting for justice, dignity, and opportunity for all Kenyans
      </p>
    </div>

    <!-- Intro Section -->
    <div class="bg-gradient-to-r from-[#202654] to-[#BC361D] text-white py-[80px] px-[20px]">
      <div class="max-w-[1200px] mx-auto text-center">
        <p class="text-[18px] md:text-[20px] max-w-[800px] mx-auto leading-relaxed">
          Fighting Brutality & Impunity (FBI) is a citizen-led movement committed to transforming Kenya into a nation where justice prevails,
          human rights are protected, and opportunity is accessible to all.
        </p>
      </div>
    </div>

    <!-- Our Story Section -->
    <div class="py-[60px] px-[20px] bg-white">
      <div class="max-w-[1200px] mx-auto">
        <div class="w-full text-center mb-[40px] relative">
          <div class="text-[#202654] font-bold text-[28px] md:text-[36px] relative z-10 inline-block px-[20px]">
            <span class="bg-white px-[15px]">Our Story</span>
          </div>
          <div class="absolute top-1/2 left-0 w-full h-[2px] bg-gradient-to-r from-transparent via-[#BC361D] to-transparent z-0"></div>
        </div>
        <div class="grid md:grid-cols-2 gap-[40px] items-center">
          <div>
            <p class="mb-[20px] text-gray-700 leading-relaxed">
              FBI Kenya was founded in 2020 by a coalition of business leaders,
              activists, and ordinary citizens who had reached breaking point
              with Kenya's systemic brutality and impunity. The movement emerged
              from the streets during nationwide protests against police
              violence and economic oppression.
            </p>
            <p class="mb-[20px] text-gray-700 leading-relaxed">
              Our formation was catalyzed by three urgent crises: (1) Rampant
              extrajudicial killings by security forces, (2) Small businesses
              being crushed by corrupt taxation systems, and (3) Youth
              unemployment reaching 70% despite Kenya's $27 trillion in natural
              resource wealth being looted by elites.
            </p>
            <div class="bg-[#BC361D] bg-opacity-10 p-[20px] border-l-4 border-[#BC361D]">
              <p class="text-[#202654] italic font-medium">
                "We are not politicians - we are citizens who refuse to watch
                Kenya's potential be stolen through brutality and impunity. Our
                movement grows daily because Kenyans are ready to fight for the
                nation we deserve."
              </p>
              <p class="mt-2 font-semibold">- FBI Kenya Founding Members</p>
            </div>
          </div>
          <div class="relative rounded-xl overflow-hidden shadow-lg h-[350px] bg-gray-100 flex items-center justify-center">
            <img src="/about.png" alt="FBI Kenya founders at first protest" class="w-full h-full object-cover">
          </div>
        </div>
      </div>
    </div>

    <!-- Mission & Vision Section -->
    <div class="py-[60px] px-[20px] bg-[#FAFAFA]">
      <div class="max-w-[1200px] mx-auto">
        <div class="w-full text-center mb-[40px] relative">
          <div class="text-[#202654] font-bold text-[28px] md:text-[36px] relative z-10 inline-block px-[20px]">
            <span class="bg-[#FAFAFA] px-[15px]">Mission & Vision</span>
          </div>
          <div class="absolute top-1/2 left-0 w-full h-[2px] bg-gradient-to-r from-transparent via-[#BC361D] to-transparent z-0"></div>
        </div>
        <div class="grid md:grid-cols-2 gap-[30px]">
          <MissionVisionCard
            title="Our Mission"
            icon="ph:target"
            :dark="true"
          >
            <p class="mb-[15px]">
              To dismantle brutality and impunity in all forms through:
            </p>
            <ul class="list-disc pl-[20px] space-y-[10px]">
              <li>Exposing corruption and human rights violations</li>
              <li>Mobilizing citizens to demand accountability</li>
              <li>Providing legal support to victims of state violence</li>
              <li>Advocating for policy reforms that protect dignity</li>
              <li>Building alternative systems of justice and opportunity</li>
            </ul>
          </MissionVisionCard>

          <MissionVisionCard
            title="Our Vision"
            icon="ph:eye"
            :dark="false"
          >
            <p>A Kenya where:</p>
            <ul class="list-disc pl-[20px] space-y-[10px] mt-[10px]">
              <li>Justice prevails over impunity</li>
              <li>Dignity is protected for all citizens</li>
              <li>Prosperity is shared, not looted</li>
              <li>Youth lead rather than languish</li>
              <li>Businesses thrive without harassment</li>
              <li>Security forces protect rather than oppress</li>
            </ul>
          </MissionVisionCard>
        </div>
      </div>
    </div>

    <!-- Who We Stand With Section -->
    <div class="py-[60px] px-[20px] bg-white">
      <div class="max-w-[1200px] mx-auto">
        <div class="w-full text-center mb-[40px] relative">
          <div class="text-[#202654] font-bold text-[28px] md:text-[36px] relative z-10 inline-block px-[20px]">
            <span class="bg-white px-[15px]">Who We Stand With</span>
          </div>
          <div class="absolute top-1/2 left-0 w-full h-[2px] bg-gradient-to-r from-transparent via-[#BC361D] to-transparent z-0"></div>
        </div>
        <div class="grid md:grid-cols-2 gap-[30px]">
          <StandWithCard
            title="Battled Business Community"
            icon="ph:storefront"
            :redTitle="true"
          >
            <p class="mb-[15px] text-gray-700">
              We stand with Kenyan entrepreneurs facing:
            </p>
            <ul class="list-disc pl-[20px] space-y-[10px]">
              <li>Punitive taxation consuming 60% of profits</li>
              <li>Corrupt licensing and inspection regimes</li>
              <li>Cartel-controlled markets</li>
              <li>Lack of access to affordable credit</li>
              <li>Constant harassment from corrupt officials</li>
            </ul>
            <p class="mt-[15px] text-gray-700">
              Our Business Defense Program provides legal support, policy
              advocacy, and corruption exposure.
            </p>
          </StandWithCard>

          <StandWithCard
            title="Betrayed Youth"
            icon="ph:users"
            :redTitle="false"
          >
            <p class="mb-[15px] text-gray-700">
              We fight for Kenya's youth facing:
            </p>
            <ul class="list-disc pl-[20px] space-y-[10px]">
              <li>70% unemployment despite education</li>
              <li>Political manipulation during elections</li>
              <li>Police brutality during protests</li>
              <li>No access to startup capital</li>
              <li>Marginalization in decision-making</li>
            </ul>
            <p class="mt-[15px] text-gray-700">
              Our Youth Empowerment Program offers skills training, startup
              incubators, and leadership development.
            </p>
          </StandWithCard>
        </div>
      </div>
    </div>

    <!-- Get Involved Section -->
    <div class="py-[60px] px-[20px] bg-[#FAFAFA]">
      <div class="max-w-[1200px] mx-auto">
        <div class="w-full text-center mb-[40px] relative">
          <div class="text-[#202654] font-bold text-[28px] md:text-[36px] relative z-10 inline-block px-[20px]">
            <span class="bg-[#FAFAFA] px-[15px]">Get Involved</span>
          </div>
          <div class="absolute top-1/2 left-0 w-full h-[2px] bg-gradient-to-r from-transparent via-[#BC361D] to-transparent z-0"></div>
        </div>
        <div class="grid md:grid-cols-3 gap-[25px]">
          <GetInvolvedCard
            title="Become a Member"
            icon="ph:user-plus"
            buttonText="Register Now"
            :borderRed="true"
            :iconRed="true"
            :outline="false"
          >
            <p class="text-gray-600 mb-[20px]">
              Join our nationwide network of changemakers. Membership gives you access to:
            </p>
            <ul class="text-left list-disc pl-[20px] space-y-[10px] mb-[20px] text-gray-700 text-[15px]">
              <li>Local chapter meetings and actions</li>
              <li>Legal protection network</li>
              <li>Business support programs</li>
              <li>Leadership training</li>
            </ul>
          </GetInvolvedCard>

          <GetInvolvedCard
            title="Volunteer"
            icon="ph:hand-heart"
            buttonText="Volunteer Today"
            :borderRed="false"
            :iconRed="false"
            :outline="true"
          >
            <p class="text-gray-600 mb-[20px]">
              Offer your skills to critical areas:
            </p>
            <ul class="text-left list-disc pl-[20px] space-y-[10px] mb-[20px] text-gray-700 text-[15px]">
              <li>Legal advocacy and paralegal support</li>
              <li>Investigative journalism and media</li>
              <li>Community organizing and mobilization</li>
              <li>Graphic design and digital campaigns</li>
              <li>Fundraising and grant writing</li>
            </ul>
          </GetInvolvedCard>

          <GetInvolvedCard
            title="Donate"
            icon="ph:currency-dollar"
            buttonText="Donate Now"
            :borderRed="true"
            :iconRed="true"
            :outline="false"
          >
            <p class="text-gray-600 mb-[20px]">Your contributions fund:</p>
            <ul class="text-left list-disc pl-[20px] space-y-[10px] mb-[20px] text-gray-700 text-[15px]">
              <li>Corruption investigations and legal actions</li>
              <li>Protection for whistleblowers and activists</li>
              <li>Youth skills training programs</li>
              <li>Business advocacy initiatives</li>
              <li>Community mobilization efforts</li>
            </ul>
          </GetInvolvedCard>
        </div>
      </div>
    </div>

    
   
  </div>
</template>