<template>
  <div class="main-content">
    <div class="container">

      <!-- Timeline with Images -->
      <div class="timeline-container">
        <!-- Timeline Line -->
        <div class="timeline-line"></div>
        
        <!-- Timeline Items -->
        <div class="timeline-item">
          <div class="timeline-marker">2010</div>
          <div class="timeline-content-wrapper">
            <div class="timeline-image">
              <img src="/ppv-paste.jpg" alt="PPV Paste" class="timeline-img" />
            </div>
            <div class="timeline-content">
              <h3>Company Founded</h3>
              <p>PLANT PV was founded by 
                <a href="https://www.linkedin.com/in/craig-peters-7134835/" target="_blank" rel="noopener">Craig Peters</a> 
                and 
                <a href="https://www.linkedin.com/in/brian-hardin-930813/" target="_blank" rel="noopener">Brian Hardin</a>
                to develop, manufacture and market photovoltaic cell materials.</p>
            </div>
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-marker">2015</div>
          <div class="timeline-content-wrapper alternate">
            <div class="timeline-content">
              <h3>Technology Development</h3>
              <p>PLANT PV developed a novel "silver-on-aluminum" solar cell metallization paste.</p>
            </div>
            <div class="timeline-image">
              <img src="/ppv-screen-printer.jpg" alt="PPV Screen Printer" class="timeline-img" />
            </div>
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-marker">2018</div>
          <div class="timeline-content-wrapper">
            <div class="timeline-image">
              <img src="/ppv-furnace.jpg" alt="PPV Furnace" class="timeline-img" />
            </div>
            <div class="timeline-content">
              <h3>Efficiency Achievement</h3>
              <p>We demonstrated a 0.1% absolute efficiency gain when our paste was applied to commercial silicon solar cells and passed TUV certification as a reliable module-level material.</p>
            </div>
          </div>
        </div>

        <div class="timeline-item">
          <div class="timeline-marker">2019</div>
          <div class="timeline-content-wrapper alternate">
            <div class="timeline-content">
              <h3>Strategic Acquisition</h3>
              <p>Our technology was acquired by a Japanese multinational materials company.</p>
            </div>
            <div class="timeline-image">
              <img src="/ppv-wafer.jpg" alt="PPV Wafer" class="timeline-img" />
            </div>
          </div>
        </div>
      </div>

      <!-- Thank You Image -->
      <div class="thank-you-section">
        <div class="thank-you-image">
          <img src="/ppv-thank-you-wafer.jpg" alt="Thank You - PPV Wafer" class="thank-you-img" />
        </div>
      </div>

    </div>
  </div>
</template>

<script setup lang="ts">
</script>

<style scoped>
.main-content {
  background: #fff;
  padding: 0.5rem 0;
}

.container {
  max-width: 1140px;
  margin: 0 auto;
  padding: 0 15px;
}


/* Timeline Styles */
.timeline-container {
  position: relative;
  max-width: 1200px;
  margin: 0.5rem auto;
  padding: 1rem 0 2rem 6rem;
}

.timeline-line {
  position: absolute;
  left: calc(6rem - 2px);
  top: 0;
  bottom: 0;
  width: 4px;
  background: linear-gradient(to bottom, #1e3a8a, #1e40af);
  z-index: 1;
}

.timeline-item {
  position: relative;
  margin-bottom: 4rem;
  padding-left: 2rem;
}

.timeline-marker {
  background: #1e3a8a;
  color: white;
  border-radius: 50%;
  width: 80px;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
  font-size: 1.1rem;
  position: absolute;
  left: -2rem;
  top: 50%;
  transform: translateY(-50%);
  z-index: 4;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
}

.timeline-content-wrapper {
  display: flex;
  gap: 2rem;
  align-items: center;
}

.timeline-content-wrapper.alternate {
  flex-direction: row-reverse;
}

.timeline-image {
  flex: 0 0 350px;
}

.timeline-img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  border-radius: 12px;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.timeline-img:hover {
  transform: scale(1.02);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
}

.timeline-content {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.1);
  flex: 1;
  border: 2px solid #e1e5e9;
  text-align: left;
  position: relative;
  z-index: 3;
  min-height: 200px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.timeline-content h3 {
  color: #1e3a8a;
  font-size: 1.4rem;
  font-weight: 600;
  margin-bottom: 1rem;
}

.timeline-content p {
  line-height: 1.6;
  margin-bottom: 0;
  font-size: 1rem;
}

/* Thank You Section */
.thank-you-section {
  margin-top: 3rem;
  text-align: center;
  padding: 0 2rem;
}

.thank-you-image {
  width: 60vw;
  max-width: 800px;
  min-width: 300px;
  margin: 0 auto;
}

.thank-you-img {
  width: 100%;
  height: auto;
  border-radius: 12px;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.thank-you-img:hover {
  transform: scale(1.02);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
}

@media (max-width: 768px) {
  .timeline-container {
    padding: 0.5rem 0.5rem 2rem 3.5rem;
    max-width: 100%;
  }
  
  .timeline-line {
    left: calc(3.5rem - 2px);
  }
  
  .timeline-item {
    padding-left: 1rem;
    margin-bottom: 3rem;
  }
  
  .timeline-marker {
    left: -1rem;
    width: 60px;
    height: 60px;
    font-size: 1rem;
  }
  
  .timeline-content-wrapper {
    flex-direction: column !important;
    gap: 1rem;
  }
  
  .timeline-content-wrapper.alternate {
    flex-direction: column !important;
  }
  
  .timeline-image {
    flex: none;
    width: 100%;
    max-width: 100%;
    margin: 0;
  }
  
  .timeline-img {
    height: 220px;
    width: 100%;
    border-radius: 8px;
  }
  
  .timeline-content {
    min-height: auto;
    padding: 1.25rem;
    margin: 0;
  }
  
  .timeline-content h3 {
    font-size: 1.3rem;
    margin-bottom: 0.75rem;
  }
  
  .timeline-content p {
    font-size: 0.95rem;
    line-height: 1.5;
  }
  
  .thank-you-section {
    margin-top: 2rem;
    padding: 0 0.5rem;
  }
}

@media (max-width: 480px) {
  .main-content {
    padding: 0.25rem 0;
  }
  
  .timeline-container {
    padding: 0.25rem 0.75rem 1.5rem 2.5rem;
  }
  
  .timeline-line {
    left: calc(2.5rem - 2px);
  }
  
  .timeline-marker {
    left: -0.75rem;
    width: 50px;
    height: 50px;
    font-size: 0.85rem;
  }
  
  .timeline-item {
    padding-left: 0.75rem;
    margin-bottom: 2.5rem;
  }
  
  .timeline-content {
    padding: 1rem;
    border-radius: 8px;
  }
  
  .timeline-content h3 {
    font-size: 1.15rem;
    margin-bottom: 0.5rem;
  }
  
  .timeline-content p {
    font-size: 0.9rem;
    line-height: 1.4;
  }
  
  .timeline-img {
    height: 180px;
    border-radius: 6px;
  }
  
  .thank-you-section {
    margin-top: 1.5rem;
    padding: 0 0.75rem;
  }
}

/* Extra small phones */
@media (max-width: 360px) {
  .timeline-container {
    padding: 0.25rem 0.5rem 1.5rem 2rem;
  }
  
  .timeline-line {
    left: calc(2rem - 2px);
  }
  
  .timeline-marker {
    left: -0.5rem;
    width: 45px;
    height: 45px;
    font-size: 0.8rem;
  }
  
  .timeline-item {
    padding-left: 0.5rem;
  }
  
  .timeline-content {
    padding: 0.75rem;
  }
  
  .timeline-content h3 {
    font-size: 1.1rem;
  }
  
  .timeline-content p {
    font-size: 0.85rem;
  }
  
  .timeline-img {
    height: 160px;
  }
}
</style>