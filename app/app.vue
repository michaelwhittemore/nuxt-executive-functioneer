<script setup lang="ts">
useHead({
  title: 'Executive Functioneer',
  meta: [
    { name: 'description', content: 'This is the meta-description of the page' },
    { property: 'og:title', content: 'This is the meta-title of the page' },
    { property: 'og:description', content: 'This is the meta-description of the page' },
  ],
})
// import '~/assets/css/main.css'
</script>


<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<style>
* {
  /* reset all styles */
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body {
  margin: 0;
  padding: 0;
}
</style>
