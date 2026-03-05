<template>
    <UContainer>
        <div class="mb-4 mt-12">
          <span class="font-semibold text-lg">Hello, I'm</span>
          <h1 class="text-5xl md:text-6xl font-bold mb-2">
            {{ myInfo.name }}
          </h1>
          <div class="flex items-center">
            <h2 class="text-2xl md:text-3xl text-gray-300">
              Aspiring <span class="text-cyber-blue">SOC Analyst</span>
            </h2>
          </div>
        </div>
        
        <!-- Journey Statement -->
        <p class="text-xl text-gray-300 mb-6 leading-relaxed">
        {{ myInfo.descriptionOne }}
        </p>
        
        <!-- Key Philosophy -->
        <div class="bg-gray-800/50 p-4 rounded-lg mb-6 border-l-4 border-cyber-blue">
          <p class="text-gray-300 italic">
           {{ myInfo.descriptionTwo }}
          </p>
        </div>
        
       <UBlogPosts :posts="posts" />
  </UContainer>

</template>
<script setup lang="ts">

const myInfo = {
  name: "Ramil Bercasio",
  descriptionOne: `I built this portfolio to document my hands-on journey toward becoming a 
        Security Operations Center (SOC) Analyst. Each module card below represents 
        a specific area of SOC training that I personally studied, practiced, and 
        applied through labs, simulations, and real-world–style scenarios.`,
  descriptionTwo: `"Rather than focusing only on theory, my training emphasizes how SOC analysts 
          actually work—from detecting suspicious activity, analyzing logs, investigating 
          alerts, to making informed response decisions."` 
  }

const posts = ref([
  {
    title: 'Email & Phishing Analysis',
    description: 'Start your defensive security career...',
    image: 'https://nuxt.com/assets/blog/nuxt-icon/cover.png',
    date: '2024-11-25',
    to: '/courses/email-and-phishing-analysis'
  },
  {
    title: 'Network Traffic Analysis',
    description: 'Explore the essential SOC analyst skills...',
    image: 'https://nuxt.com/assets/blog/v3.14.png',
    date: '2024-11-04',
    to: '/courses/soc-team-internals'
  },
  {
    title: 'Network Security Monitoring',
    description: 'Explore the essential SOC analyst skills...',
    image: 'https://nuxt.com/assets/blog/v3.14.png',
    date: '2024-11-04',
    to: '/courses/soc-team-internals'
  },
  {
    title: 'Web Security Monitoring',
    description: 'Explore the essential SOC analyst skills...',
    image: 'https://nuxt.com/assets/blog/v3.14.png',
    date: '2024-11-04',
    to: '/courses/soc-team-internals'
  },
  {
    title: 'Windows Security Monitoring',
    description: 'Explore the essential SOC analyst skills...',
    image: 'https://nuxt.com/assets/blog/v3.14.png',
    date: '2024-11-04',
    to: '/courses/windows-security-monitoring'
  },
   {
    title: 'Linux Security Monitoring',
    description: 'Explore the essential SOC analyst skills...',
    image: 'https://nuxt.com/assets/blog/v3.14.png',
    date: '2024-11-04',
    to: '/courses/linux-security-monitoring'
  },
  {
    title: 'Malware Analysis',
    description: 'Explore the essential SOC analyst skills...',
    image: 'https://nuxt.com/assets/blog/v3.14.png',
    date: '2024-11-04',
    to: '/courses/soc-team-internals'
  },
   {
    title: 'Threat Analysis',
    description: 'Explore the essential SOC analyst skills...',
    image: 'https://nuxt.com/assets/blog/v3.14.png',
    date: '2024-11-04',
    to: '/courses/threat-analysis'
  },
   {
    title: 'SIEM Triage for SOC with Splunk',
    description: 'Explore the essential SOC analyst skills...',
    image: '/splunk/splunkLogo.png',
    date: '2024-11-04',
    to: '/labs/siem-triage-for-soc'
  },
  {
    title: 'SIEM Triage for SOC with Splunk',
    description: 'Explore the essential SOC analyst skills...',
    image: '/splunk/splunkLogo.png',
    date: '2024-11-04',
    to: '/siem-triage-for-soc'
  },

])



</script>


  //  {
  //   title: 'SIEM Triage for SOC with Elastic',
  //   description: 'Explore the essential SOC analyst skills...',
  //   image: 'https://nuxt.com/assets/blog/v3.14.png',
  //   date: '2024-11-04',
  //   to: '/courses/siem-triage-for-soc'
  // }




    <!-- <div class="my-8">
         <p class="">
        Ramil Bercasio
      </p>
      <p class="text-muted">
  SOC Analyst Trainee
      </p>
    </div>
    
    <div class="my-8">
    <p>SOC Training Portfolio</p>
     <p class="text-muted text-center text-2xl">
      I built this portfolio to document my hands-on journey toward becoming a Security Operations Center (SOC) Analyst. Each module card below represents a specific area of SOC training that I personally studied, practiced, and applied through labs, simulations, and real-world–style scenarios.

Rather than focusing only on theory, my training emphasizes how SOC analysts actually work—from detecting suspicious activity, analyzing logs, investigating alerts, to making informed response decisions.

This portfolio demonstrates my ability to think like a defender, understand attacker behavior, and apply structured analysis using industry-standard frameworks and tools.
    </p>
    </div> -->