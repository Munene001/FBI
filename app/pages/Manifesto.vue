<template>
<div class="bg-[#FAFAFA] min-h-screen pb-[60px] font-[uno]">
    <!-- Hero Section -->
    <div class="bg-gradient-to-r from-[#202654] to-[#BC361D] text-white  py-[80px] md:pt-[138px] px-[20px] text-center">
      <h1 class="text-[36px] md:text-[48px] font-bold mb-[20px]">FBI Kenya Manifesto</h1>
      <p class="text-[18px] max-w-[800px] mx-auto">
        Our comprehensive blueprint for dismantling brutality and impunity in Kenya
      </p>
    </div>

    <div class="max-w-[1200px] mx-auto px-[20px]">
      <!-- Ecosystem of Brutality Section -->
      <div class="py-[60px]">
        <ManifestoSection title="Kenya's Reality: The Ecosystem of Brutality" />
        
        <div class="grid md:grid-cols-3 gap-[30px]">
          <!-- Economic Brutality -->
          <PrincipleCard 
            title="Economic Brutality" 
            icon="ph:currency-circle-dollar" 
            :redTitle="true"
          >
            <ul class="list-disc pl-[20px] space-y-[10px] text-gray-700">
              <li>Excessive taxation consuming up to 60% of business profits</li>
              <li>70% youth unemployment despite education</li>
              <li>Farmers exploited by cartels in tea, coffee, and dairy sectors</li>
              <li>Small businesses crushed by corrupt licensing systems</li>
              <li>$27 trillion in natural resources looted by elites</li>
            </ul>
          </PrincipleCard>

          <!-- Social Brutality -->
          <PrincipleCard 
            title="Social Brutality" 
            icon="game-icons:brutal-helm" 
            :redTitle="false"
          >
            <ul class="list-disc pl-[20px] space-y-[10px] text-gray-700">
              <li>Police killings and extrajudicial executions</li>
              <li>Gender-based violence and discrimination</li>
              <li>Marginalized communities denied basic services</li>
              <li>Crumbling healthcare and education systems</li>
              <li>Persons with disabilities facing systemic exclusion</li>
            </ul>
          </PrincipleCard>

          <!-- Political & Governance -->
          <PrincipleCard 
            title="Political Brutality" 
            icon="ri:criminal-fill" 
            :redTitle="true"
          >
            <ul class="list-disc pl-[20px] space-y-[10px] text-gray-700">
              <li>Grand corruption in government deals</li>
              <li>Opaque contracts for natural resources</li>
              <li>Shrinking civic space and protest rights</li>
              <li>Weaponization of security agencies</li>
              <li>Political betrayal of youth and businesses</li>
            </ul>
          </PrincipleCard>
        </div>
      </div>

      <!-- People's Charter Section -->
      <div class="py-[60px] bg-white rounded-xl p-[30px]">
        <ManifestoSection title="The People's Charter" />
        
        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-[20px]">
          <PrincipleCard
            title="Enforced Governance"
            icon="ph:scroll"
            :redTitle="false"
          >
            Full adherence to Kenya's Constitution with consequences for violations
          </PrincipleCard>

          <PrincipleCard
            title="Transparency & Accountability"
            icon="icons8:binoculars"
            :redTitle="true"
          >
            Mandatory public audits and open contracting in all government dealings
          </PrincipleCard>

          <PrincipleCard
            title="Zero Tolerance for Corruption"
            icon="ant-design:stop-filled"
            :redTitle="false"
          >
            Immediate prosecution of corrupt officials with asset recovery
          </PrincipleCard>

          <PrincipleCard
            title="Justice & Fairness"
            icon="mdi:justice"
            :redTitle="true"
          >
            Living wages and equitable resource distribution for all Kenyans
          </PrincipleCard>

          <PrincipleCard
            title="Human Rights & Dignity"
            icon="ph:heart"
            :redTitle="false"
          >
            Protection of all constitutional rights including gender equality
          </PrincipleCard>

          <PrincipleCard
            title="Security Sector Reform"
            icon="ph:shield-check"
            :redTitle="true"
          >
            Professional, well-trained security forces with civilian oversight
          </PrincipleCard>

          <PrincipleCard
            title="Business & Youth Support"
            icon="streamline-pixel:business-products-performance-money-increase"
            :redTitle="false"
          >
            Tax reforms and policies enabling entrepreneurs and youth to thrive
          </PrincipleCard>

          <PrincipleCard
            title="Resource Sovereignty"
            icon="ph:globe"
            :redTitle="true"
          >
            Kenya's natural wealth must benefit all citizens first
          </PrincipleCard>
        </div>
      </div>

      <!-- Strategic Action Plan -->
      <div class="py-[60px]">
        <ManifestoSection title="Strategic Action Plan" />
        
        <div class="space-y-[30px]">
          <ActionPlanCard
            number="1"
            title="Expose & Dismantle Impunity"
            :actions="[
              'Launch investigations into corruption and abuse cases',
              'Strengthen judicial institutions with citizen oversight',
              'Support victims and whistleblowers with legal protection'
            ]"
          />

          <ActionPlanCard
            number="2"
            title="Empower Citizens, Business & Youth"
            :actions="[
              'Nationwide civic education on constitutional rights',
              'Develop leadership programs for marginalized groups',
              'Create business-friendly policies and access to finance'
            ]"
          />

          <ActionPlanCard
            number="3"
            title="Protect Farmers, Workers & Business"
            :actions="[
              'Campaign for fair trade policies and transparent markets',
              'Advocate for living wages and safe working conditions',
              'Support sustainable agricultural practices'
            ]"
          />

          <ActionPlanCard
            number="4"
            title="Safeguard Natural Resources"
            :actions="[
              'Push for full transparency in resource extraction',
              'Strengthen environmental protection laws',
              'Combat illegal logging and land grabbing'
            ]"
          />

          <ActionPlanCard
            number="5"
            title="Accelerate Growth & Youth Opportunities"
            :actions="[
              'Establish industrial parks and innovation hubs',
              'Support youth-led startups and community projects',
              'Promote skills training and mentorship programs'
            ]"
          />

          <ActionPlanCard
            number="6"
            title="Defend Civil Liberties & Rights"
            :actions="[
              'Protect freedom of speech and peaceful protest',
              'Challenge laws threatening democratic space',
              'Provide legal aid to activists and journalists'
            ]"
          />
        </div>
      </div>

      <!-- Ongoing Campaigns -->
      <div class="py-[60px]">
        <ManifestoSection title="Ongoing Campaigns" />
        
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-[30px]">
          <CampaignCard
            title="Justice & Anti-Corruption"
            icon="streamline:justice-hammer-solid"
            description="Exposing looting and fighting impunity at all levels"
            :items="[
              'Corruption case investigations',
              'Asset recovery initiatives',
              'Judicial reforms advocacy'
            ]"
          />

          <CampaignCard
            title="Betrayed Youth Movement"
            icon="material-symbols:campaign-outline-rounded"
            description="Creating real opportunities for Kenya's youth"
            :items="[
              'Skills training programs',
              'Startup incubators',
              'Leadership development'
            ]"
          />

          <CampaignCard
            title="Business Community Defense"
            icon="material-symbols-light:business-center"
            description="Protecting entrepreneurs from exploitation"
            :items="[
              'Policy advocacy',
              'Legal support',
              'Corruption exposure'
            ]"
          />
        </div>
      </div>
    </div>
  </div>
</template>