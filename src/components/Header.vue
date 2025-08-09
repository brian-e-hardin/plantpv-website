<template>
  <header class="header">
    <div class="container">
      <div class="logo">
        <img src="/plant-pv-logo.jpg" alt="Plant PV" class="logo-image" />
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">
</script>

<style scoped>
.header {
  background: var(--background);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 1rem 0;
  position: sticky;
  top: 0;
  z-index: 100;
}

.logo {
  text-align: center;
}

.logo-image {
  height: 60px;
  width: auto;
  max-width: 100%;
  object-fit: contain;
}

@media (max-width: 768px) {
  .logo-image {
    height: 45px;
  }
}
</style>