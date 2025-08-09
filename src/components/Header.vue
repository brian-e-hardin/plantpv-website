<template>
  <header class="header">
    <div class="container">
      <div class="logo">
        <h1>Plant PV</h1>
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

.logo h1 {
  color: var(--primary-blue);
  font-size: 2rem;
  font-weight: 700;
  text-align: center;
}

@media (max-width: 768px) {
  .logo h1 {
    font-size: 1.5rem;
  }
}
</style>