<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-content">
        <p>&copy; {{ currentYear }} Plant PV. All rights reserved.</p>
        <p class="footer-description">
          Advancing solar technology through innovative metallization solutions.
        </p>
      </div>
    </div>
  </footer>
</template>

<script setup lang="ts">
import { computed } from 'vue'

const currentYear = computed(() => new Date().getFullYear())
</script>

<style scoped>
.footer {
  background: var(--text-primary);
  color: white;
  padding: 2rem 0;
  margin-top: auto;
}

.footer-content {
  text-align: center;
}

.footer-content p {
  margin-bottom: 0.5rem;
  opacity: 0.9;
}

.footer-description {
  font-size: 0.9rem;
  opacity: 0.7;
}

@media (max-width: 768px) {
  .footer {
    padding: 1.5rem 0;
  }
  
  .footer-content p {
    font-size: 0.9rem;
  }
  
  .footer-description {
    font-size: 0.8rem;
  }
}
</style>