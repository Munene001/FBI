<template>
 <Carousel/>
  <SectionWrapper
    title="Our Fight For Kenya"
    subtitle="We're building a movement to transform our nation's future"
    :light="true"
  >
    <div class="grid md:grid-cols-2 gap-[40px] items-center">
      <div>
        <div class="text-[#BC361D] text-[20px] font-bold mb-[15px]">
          WHO WE ARE
        </div>
        <h2 class="text-[32px] font-bold text-[#202654] mb-[20px]">
          Citizens United Against Brutality & Impunity
        </h2>
        <p class="text-[18px] text-gray-700 mb-[30px]">
          FBI Kenya is a citizen-led movement committed to transforming Kenya
          into a nation where justice prevails, human rights are protected, and
          opportunity is accessible to all.
        </p>
        <div
          class="bg-[#FAFAFA] border-l-4 border-[#BC361D] p-[25px] mb-[30px]"
        >
          <p class="italic text-[18px] text-[#202654]">
            "We are ordinary Kenyans from all walks of life who have said ENOUGH
            to the systemic oppression holding our nation back."
          </p>
        </div>
        <NuxtLink
          to="/about"
          class="inline-flex items-center text-[#BC361D] font-bold group"
        >
          Discover our full story
          <Icon
            name="ph:arrow-right"
            class="ml-[8px] group-hover:translate-x-2 transition-transform"
          />
        </NuxtLink>
      </div>
      <div class="relative h-[400px] rounded-2xl overflow-hidden shadow-xl">
        <img
          src="/c.jpg"
          alt="FBI Kenya community action"
          class="w-full h-full object-cover"
        />
        <div
          class="absolute bottom-0 left-0 w-full p-[30px] bg-gradient-to-t from-black/80 to-transparent"
        >
          <div class="text-white text-[14px]">Nairobi, 2024</div>
        </div>
      </div>
    </div>
  </SectionWrapper>

  <!-- The Brutality We Fight Section -->
  <SectionWrapper
    title="The Brutality We Fight"
    subtitle="Systemic injustices crushing Kenya's potential"
    :light="false"
  >
    <div class="grid md:grid-cols-3 gap-[30px]">
      <!-- Economic Oppression Card -->
      <BrutalityCard
        icon="ph:currency-circle-dollar"
        link="/manifesto#economic"
        :red-icon="true"
      >
        <template #title>Economic Oppression</template>
        <template #content>
          <ul class="space-y-[12px]">
            <li class="flex items-start gap-[10px]">
              <div class="text-[#BC361D]">•</div>
              <div>70% youth unemployment</div>
            </li>
            <li class="flex items-start gap-[10px]">
              <div class="text-[#BC361D]">•</div>
              <div>Businesses crushed by taxes</div>
            </li>
            <li class="flex items-start gap-[10px]">
              <div class="text-[#BC361D]">•</div>
              <div>$27 trillion resources looted</div>
            </li>
          </ul>
        </template>
        <template #link-text>See economic details</template>
      </BrutalityCard>

      <!-- Social Injustice Card -->
      <BrutalityCard
        icon="game-icons:brutal-helm"
        link="/manifesto#social"
        :red-icon="false"
      >
        <template #title>Social Injustice</template>
        <template #content>
          <ul class="space-y-[12px]">
            <li class="flex items-start gap-[10px]">
              <div class="text-[#BC361D]">•</div>
              <div>Police brutality & killings</div>
            </li>
            <li class="flex items-start gap-[10px]">
              <div class="text-[#BC361D]">•</div>
              <div>Crumbling public services</div>
            </li>
            <li class="flex items-start gap-[10px]">
              <div class="text-[#BC361D]">•</div>
              <div>Marginalized communities</div>
            </li>
          </ul>
        </template>
      </BrutalityCard>

      <!-- Political Corruption Card -->
      <BrutalityCard
        icon="ri:criminal-fill"
        link="/manifesto#political"
        :red-icon="true"
      >
        <template #title>Political Corruption</template>
        <template #content>
          <ul class="space-y-[12px]">
            <li class="flex items-start gap-[10px]">
              <div class="text-[#BC361D]">•</div>
              <div>Grand corruption schemes</div>
            </li>
            <li class="flex items-start gap-[10px]">
              <div class="text-[#BC361D]">•</div>
              <div>Secret resource deals</div>
            </li>
            <li class="flex items-start gap-[10px]">
              <div class="text-[#BC361D]">•</div>
              <div>Weaponized institutions</div>
            </li>
          </ul>
        </template>
      </BrutalityCard>
    </div>
  </SectionWrapper>

  <!-- Our Guiding Principles Section -->

  <SectionWrapper
    title="Our Guiding Principles"
    subtitle="The foundation of everything we fight for"
    :light="false"
  >
    <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-[30px]">
      <!-- Principle 1 -->
      <HomePrincipleCard icon="ph:hand" :dark="true">
        <template #title>Zero Tolerance for Corruption</template>
        <template #description>
          Immediate prosecution of corrupt officials with asset recovery
        </template>
      </HomePrincipleCard>

      <!-- Principle 2 -->
      <HomePrincipleCard icon="mdi:justice" :dark="false">
        <template #title>Justice & Fairness</template>
        <template #description>
          Equitable systems that protect all Kenyans equally
        </template>
      </HomePrincipleCard>

      <!-- Principle 3 -->
      <HomePrincipleCard icon="ph:binoculars" :dark="true">
        <template #title>Transparency</template>
        <template #description>
          Open governance and access to information in all dealings
        </template>
      </HomePrincipleCard>

      <!-- Principle 4 -->
      <HomePrincipleCard icon="ph:rocket" :dark="false">
        <template #title>Youth Empowerment</template>
        <template #description>
          Creating real opportunities for Kenya's next generation
        </template>
      </HomePrincipleCard>
    </div>
  </SectionWrapper>

  <!-- Call to Action Section -->
  <CTASection
    title="Ready to join the fight for Kenya's future?"
    subtitle="Whether you can volunteer, donate, or simply spread awareness - every action counts in our movement."
  >
    <NuxtLink
      to="/join"
      class="bg-[#BC361D] hover:bg-[#d94126] text-white px-[40px] py-[18px] rounded-full font-bold text-[18px] transition-colors flex items-center gap-[10px]"
    >
      <Icon name="ph:user-plus" /> Become a Member
    </NuxtLink>
    <NuxtLink
      to="/donate"
      class="bg-white hover:bg-gray-100 text-[#202654] px-[40px] py-[18px] rounded-full font-bold text-[18px] transition-colors flex items-center gap-[10px]"
    >
      <Icon name="ph:heart" /> Support Financially
    </NuxtLink>
  </CTASection>
</template>

