<template>
  <section class="timeline-section">
    <div class="container">
      <h2>Company Timeline</h2>
      <div class="timeline">
        <div class="timeline-item" v-for="item in timelineData" :key="item.year">
          <div class="timeline-year">{{ item.year }}</div>
          <div class="timeline-content">
            <h3>{{ item.title }}</h3>
            <p>{{ item.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
interface TimelineItem {
  year: string;
  title: string;
  description: string;
}

const timelineData: TimelineItem[] = [
  {
    year: "2010",
    title: "Company Founded",
    description: "Plant PV was established with a vision to revolutionize solar cell technology through innovative metallization solutions."
  },
  {
    year: "2015",
    title: "Technology Development",
    description: "Breakthrough in developing silver-on-aluminum solar cell metallization paste, focusing on improving electrical conductivity and reducing manufacturing costs."
  },
  {
    year: "2018",
    title: "Efficiency Achievement",
    description: "Successfully achieved 0.1% efficiency improvement in photovoltaic systems, representing a significant advancement in solar technology."
  },
  {
    year: "2019",
    title: "Strategic Acquisition",
    description: "Plant PV was acquired by a leading Japanese multinational corporation, enabling global scale and enhanced research capabilities."
  }
]
</script>

<style scoped>
.timeline-section {
  padding: 4rem 0;
  background: var(--light-gray);
}

.timeline-section h2 {
  text-align: center;
  font-size: 2.5rem;
  font-weight: 700;
  color: var(--text-primary);
  margin-bottom: 3rem;
}

.timeline {
  position: relative;
  max-width: 800px;
  margin: 0 auto;
}

.timeline::before {
  content: '';
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  width: 3px;
  height: 100%;
  background: var(--primary-blue);
}

.timeline-item {
  display: flex;
  align-items: center;
  margin-bottom: 3rem;
  position: relative;
}

.timeline-item:nth-child(odd) {
  justify-content: flex-end;
}

.timeline-item:nth-child(odd) .timeline-content {
  text-align: right;
  margin-right: 2rem;
}

.timeline-item:nth-child(even) .timeline-content {
  text-align: left;
  margin-left: 2rem;
}

.timeline-year {
  background: var(--primary-blue);
  color: white;
  border-radius: 50%;
  width: 80px;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.1rem;
  font-weight: 700;
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  z-index: 2;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.timeline-content {
  background: white;
  padding: 2rem;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  max-width: 350px;
  border: 1px solid var(--border-gray);
}

.timeline-content h3 {
  color: var(--primary-blue);
  font-size: 1.5rem;
  font-weight: 600;
  margin-bottom: 1rem;
}

.timeline-content p {
  color: var(--text-secondary);
  line-height: 1.6;
}

@media (max-width: 768px) {
  .timeline-section {
    padding: 2.5rem 0;
  }
  
  .timeline-section h2 {
    font-size: 2rem;
    margin-bottom: 2rem;
  }
  
  .timeline::before {
    left: 30px;
  }
  
  .timeline-item {
    justify-content: flex-start !important;
    padding-left: 80px;
  }
  
  .timeline-item:nth-child(odd) .timeline-content,
  .timeline-item:nth-child(even) .timeline-content {
    text-align: left;
    margin: 0;
  }
  
  .timeline-year {
    left: 30px;
    transform: translateX(-50%);
    width: 60px;
    height: 60px;
    font-size: 0.9rem;
  }
  
  .timeline-content {
    max-width: none;
    margin-left: 1rem;
  }
}

@media (max-width: 480px) {
  .timeline-content {
    padding: 1.5rem;
  }
  
  .timeline-content h3 {
    font-size: 1.25rem;
  }
}
</style>