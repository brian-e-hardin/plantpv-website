<template>
  <div class="main-content-section">
    <!-- Introduction -->
    <div class="intro-section">
      <p>
        Plant PV was founded in 2010 by 
        <a href="https://www.linkedin.com/in/craig-peters-7134835/" target="_blank" rel="noopener">Craig Peters</a> 
        and 
        <a href="https://www.linkedin.com/in/brian-hardin-930813/" target="_blank" rel="noopener">Brian Hardin</a>
        to develop, manufacture and market photovoltaic cell materials.
      </p>
    </div>

    <!-- Images Grid -->
    <div class="images-grid">
      <div class="image-item">
        <img src="/ppv-paste-1.jpg" alt="PPV Paste" class="content-image" />
      </div>
      <div class="image-item">
        <img src="/ppv-furnace.jpg" alt="PPV Furnace" class="content-image" />
      </div>
      <div class="image-item">
        <img src="/ppv-wafer.jpg" alt="PPV Wafer" class="content-image" />
      </div>
    </div>

    <!-- Timeline Content -->
    <div class="timeline-content">
      <div class="timeline-item">
        <h3>2015</h3>
        <p>
          Plant PV developed a novel "silver-on-aluminum" solar cell metallization paste.
        </p>
      </div>

      <div class="timeline-item">
        <h3>2018</h3>
        <p>
          We demonstrated a 0.1% absolute efficiency gain when our paste was applied to 
          commercial silicon solar cells and passed TUV certification as a reliable 
          module-level material.
        </p>
      </div>

      <div class="timeline-item">
        <h3>2019</h3>
        <p>
          Our technology was acquired by a Japanese multinational materials company.
        </p>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
</script>

<style scoped>
.main-content-section {
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem 1rem;
}

.intro-section {
  margin-bottom: 3rem;
  font-size: 1.1rem;
  text-align: center;
}

.intro-section p {
  line-height: 1.8;
}

.images-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  margin-bottom: 3rem;
  justify-items: center;
}

.image-item {
  text-align: center;
}

.content-image {
  width: 100%;
  max-width: 300px;
  height: 200px;
  object-fit: cover;
  border-radius: 4px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.timeline-content {
  margin-top: 2rem;
}

.timeline-item {
  margin-bottom: 2rem;
  padding: 1.5rem;
  background: var(--light-gray);
  border-radius: 8px;
  border-left: 4px solid var(--primary-blue);
}

.timeline-item h3 {
  font-family: 'Oswald', sans-serif;
  font-size: 1.5rem;
  font-weight: 600;
  color: var(--primary-blue);
  margin-bottom: 1rem;
}

.timeline-item p {
  font-size: 1rem;
  line-height: 1.7;
  margin-bottom: 0;
}

@media (max-width: 768px) {
  .main-content-section {
    padding: 1rem 0.5rem;
  }
  
  .images-grid {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  
  .intro-section {
    font-size: 1rem;
    margin-bottom: 2rem;
  }
  
  .timeline-item {
    padding: 1rem;
  }
  
  .timeline-item h3 {
    font-size: 1.3rem;
  }
}

@media (max-width: 480px) {
  .content-image {
    max-width: 280px;
    height: 180px;
  }
}
</style>