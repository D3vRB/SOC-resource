<!-- <script setup lang="ts">
const route = useRoute()

const path = '/' + (route.params.slug as string[]).join('/')

const { data: page } = await useAsyncData(
  () => `${path}`,
  () => queryCollection('content').path(`${path}`).first()
)

if (!page.value) {
  throw createError({
    statusCode: 404,
    statusMessage: 'Page not found'
  })
}
</script> -->

<template>
  <div class="max-w-3xl mx-auto p-6">
    <ContentRenderer v-if="page" :value="page" />
  </div>
</template>


<script setup lang="ts">
const route = useRoute()

const slug = route.params.slug

const path = Array.isArray(slug)
  ? '/' + slug.join('/')
  : '/' + (slug || '')

const { data: page } = await useAsyncData(
  `page-${path}`,
  () => queryCollection('content').path(path).first()
)

if (!page.value) {
  throw createError({
    statusCode: 404,
    statusMessage: 'Page not found'
  })
}
</script>
