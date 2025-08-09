<template>
  <div id="app">
    <Header />
    <main class="main-content">
      <div class="container">
        <div class="content-wrapper">
          <MainContent />
        </div>
      </div>
    </main>
  </div>
</template>

<script setup lang="ts">
import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'
</script>

<style scoped>
.main-content {
  padding: 2rem 0;
}

.content-wrapper {
  background: white;
}
</style>