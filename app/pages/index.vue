<!-- <template>
  <UApp>
    <div class="flex flex-row justify-center items-center fixed px-6 py-6 w-full z-50 bg-green-800">
      <div class="flex justify-end w-7xl px-2 md:px-6">
          <UButton
            color="primary"
            variant="outline"
            to="https://github.com/nuxt/ui"
            target="_blank"
            icon="i-simple-icons-github"
            aria-label="GitHub"
            label="Open Source"
            :trailing="true"
            size="xl"
          />
      </div>
    </div>
    <UMain class="pt-24">
       <UContainer>
       <div class="my-8">
         <p class="">
        Ramil Bercasio
      </p>
      <p class="text-muted">
  SOC Analyst Trainee
      </p>
    </div>
    
    <div class="my-8">
    <p>SOC Training Portfolio</p>
     <p class="text-muted text-justify">
      I built this portfolio to document my hands-on journey toward becoming a Security Operations Center (SOC) Analyst. Each module card below represents a specific area of SOC training that I personally studied, practiced, and applied through labs, simulations, and real-world–style scenarios.

Rather than focusing only on theory, my training emphasizes how SOC analysts actually work—from detecting suspicious activity, analyzing logs, investigating alerts, to making informed response decisions.

This portfolio demonstrates my ability to think like a defender, understand attacker behavior, and apply structured analysis using industry-standard frameworks and tools.
    </p>
    </div>
       <UBlogPosts :posts="posts" />
  </UContainer>
    </UMain>
  </UApp>

</template>

<script setup lang="ts">

const posts = ref([
  {
    title: 'Email & Phishing Analysis',
    description: 'Start your defensive security career...',
    image: 'https://nuxt.com/assets/blog/nuxt-icon/cover.png',
    date: '2024-11-25',
    to: '/courses/blue-team-introduction'
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
    title: 'Windows & Linux Security Monitoring',
    description: 'Explore the essential SOC analyst skills...',
    image: 'https://nuxt.com/assets/blog/v3.14.png',
    date: '2024-11-04',
    to: '/courses/soc-team-internals'
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
    to: '/courses/soc-team-internals'
  }
])

</script> -->

<template>
    <UContainer>
       <div class="my-8">
         <p class="">
        Ramil Bercasio
      </p>
      <p class="text-muted">
  SOC Analyst Trainee
      </p>
    </div>
    
    <div class="my-8">
    <p>SOC Training Portfolio</p>
     <p class="text-muted text-justify">
      I built this portfolio to document my hands-on journey toward becoming a Security Operations Center (SOC) Analyst. Each module card below represents a specific area of SOC training that I personally studied, practiced, and applied through labs, simulations, and real-world–style scenarios.

Rather than focusing only on theory, my training emphasizes how SOC analysts actually work—from detecting suspicious activity, analyzing logs, investigating alerts, to making informed response decisions.

This portfolio demonstrates my ability to think like a defender, understand attacker behavior, and apply structured analysis using industry-standard frameworks and tools.
    </p>
    </div>
       <UBlogPosts :posts="posts" />
  </UContainer>

</template>
<script setup lang="ts">

const posts = ref([
  // {
  //   title: 'Email & Phishing Analysis',
  //   description: 'Start your defensive security career...',
  //   image: 'https://nuxt.com/assets/blog/nuxt-icon/cover.png',
  //   date: '2024-11-25',
  //   to: '/courses/email-and-phishing-analysis'
  // },
  // {
  //   title: 'Network Traffic Analysis',
  //   description: 'Explore the essential SOC analyst skills...',
  //   image: 'https://nuxt.com/assets/blog/v3.14.png',
  //   date: '2024-11-04',
  //   to: '/courses/soc-team-internals'
  // },
  // {
  //   title: 'Network Security Monitoring',
  //   description: 'Explore the essential SOC analyst skills...',
  //   image: 'https://nuxt.com/assets/blog/v3.14.png',
  //   date: '2024-11-04',
  //   to: '/courses/soc-team-internals'
  // },
  // {
  //   title: 'Web Security Monitoring',
  //   description: 'Explore the essential SOC analyst skills...',
  //   image: 'https://nuxt.com/assets/blog/v3.14.png',
  //   date: '2024-11-04',
  //   to: '/courses/soc-team-internals'
  // },
  // {
  //   title: 'Windows Security Monitoring',
  //   description: 'Explore the essential SOC analyst skills...',
  //   image: 'https://nuxt.com/assets/blog/v3.14.png',
  //   date: '2024-11-04',
  //   to: '/courses/windows-security-monitoring'
  // },
  //  {
  //   title: 'Linux Security Monitoring',
  //   description: 'Explore the essential SOC analyst skills...',
  //   image: 'https://nuxt.com/assets/blog/v3.14.png',
  //   date: '2024-11-04',
  //   to: '/courses/linux-security-monitoring'
  // },
  // {
  //   title: 'Malware Analysis',
  //   description: 'Explore the essential SOC analyst skills...',
  //   image: 'https://nuxt.com/assets/blog/v3.14.png',
  //   date: '2024-11-04',
  //   to: '/courses/soc-team-internals'
  // },
  //  {
  //   title: 'Threat Analysis',
  //   description: 'Explore the essential SOC analyst skills...',
  //   image: 'https://nuxt.com/assets/blog/v3.14.png',
  //   date: '2024-11-04',
  //   to: '/courses/threat-analysis'
  // },
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
  //  {
  //   title: 'SIEM Triage for SOC with Elastic',
  //   description: 'Explore the essential SOC analyst skills...',
  //   image: 'https://nuxt.com/assets/blog/v3.14.png',
  //   date: '2024-11-04',
  //   to: '/courses/siem-triage-for-soc'
  // }
])

</script>