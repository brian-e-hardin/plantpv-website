<template>
  <div id="app">
    <Header />
    <Hero />
    <Timeline />
    <Footer />
  </div>
</template>

<script setup lang="ts">
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Timeline from './components/Timeline.vue'
import Footer from './components/Footer.vue'
</script>

<style scoped>
#app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
</style>