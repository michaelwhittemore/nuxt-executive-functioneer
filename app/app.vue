<script setup lang="ts">
useHead({
  title: 'Executive Functioneer',
  meta: [
    { name: 'description', content: 'Decluttering for adults with ADHD' },
    { property: 'og:title', content: 'Executive Functioneer - Decluttering for adults with ADHD' },
    { property: 'og:description', content: 'Decluttering for adults with ADHD' },
    { property: 'og:image', content: 'https://executivefunctioneer.com/img/brain.png' },
  ],
  link: [
    { rel: 'preconnect', href: 'https://fonts.googleapis.com' },
    { rel: 'preconnect', href: 'https://fonts.gstatic.com', crossorigin: '' },
    { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap' },
  ],
})
import '~/assets/css/main.css'
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
  font-family: 'Inter', sans-serif;
  height: 100%;
  min-height: 100vh;
}

#__nuxt {
  height: 100%;
  min-height: 100vh;
}
</style>
