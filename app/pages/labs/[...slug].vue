<script setup lang="ts">
const route = useRoute()

const path = '/' + (route.params.slug as string[]).join('/')

const { data: page } = await useAsyncData(
  () => `labs-${path}`,
  () => queryCollection('content').path(`/labs${path}`).first()
)

if (!page.value) {
  throw createError({
    statusCode: 404,
    statusMessage: 'Page not found'
  })
}
</script>

<template>
  <div class="max-w-3xl mx-auto p-6">
    <ContentRenderer v-if="page" :value="page" />
  </div>
</template>
