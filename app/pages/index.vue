<script setup>
const config = useRuntimeConfig()
const homeURL = config.public.homeURL

if (import.meta.client && homeURL) {
  navigateTo(homeURL, { external: true })
}
</script>

<template>
  <main class="flex flex-col justify-center">
    <HomeTwitter />
    <HomeHero />
    <HomeFeatures />
    <HomeLogos />
    <HomeCta />
  </main>
</template>
