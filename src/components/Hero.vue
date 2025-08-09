<template>
  <section class="hero">
    <div class="container">
      <div class="hero-content">
        <h2>Solar Technology Innovation</h2>
        <p class="hero-description">
          Plant PV developed breakthrough solar cell metallization paste technology, 
          achieving significant efficiency improvements in photovoltaic systems.
        </p>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
</script>

<style scoped>
.hero {
  background: linear-gradient(135deg, var(--primary-blue), var(--light-blue));
  color: white;
  padding: 4rem 0;
  text-align: center;
}

.hero-content h2 {
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 1.5rem;
  line-height: 1.2;
}

.hero-description {
  font-size: 1.25rem;
  max-width: 600px;
  margin: 0 auto;
  opacity: 0.95;
  line-height: 1.6;
}

@media (max-width: 768px) {
  .hero {
    padding: 2.5rem 0;
  }
  
  .hero-content h2 {
    font-size: 2rem;
  }
  
  .hero-description {
    font-size: 1.1rem;
    padding: 0 1rem;
  }
}

@media (max-width: 480px) {
  .hero-content h2 {
    font-size: 1.75rem;
  }
  
  .hero-description {
    font-size: 1rem;
  }
}
</style>