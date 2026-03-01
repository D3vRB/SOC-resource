<script setup lang="ts">
const posts = ref([
  {
    title: 'Blue Team Introduction',
    description: 'Start your defensive security career...',
    image: 'https://nuxt.com/assets/blog/nuxt-icon/cover.png',
    date: '2024-11-25',
    to: '/courses/blue-team-introduction'
  },
  {
    title: 'SOC Team Internals',
    description: 'Explore the essential SOC analyst skills...',
    image: 'https://nuxt.com/assets/blog/v3.14.png',
    date: '2024-11-04',
    to: '/courses/soc-team-internals'
  }
])
</script>

<template>
  <UBlogPosts :posts="posts" />
</template>
