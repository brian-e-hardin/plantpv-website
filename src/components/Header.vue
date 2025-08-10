<template>
  <header class="site-header">
    <div class="container">
      <div class="site-branding">
        <a href="#" class="custom-logo-link">
          <img 
            src="/logo.jpg" 
            alt="Plant PV - New Materials for Photovoltaic Cells" 
            class="custom-logo"
          />
        </a>
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">
</script>

<style scoped>
.site-header {
  background: #fff;
  padding: 1rem 0;
}

.container {
  max-width: 1140px;
  margin: 0 auto;
  padding: 0 15px;
}

.site-branding {
  text-align: center;
}

.custom-logo-link {
  display: inline-block;
}

.custom-logo {
  height: auto;
  max-width: 400px;
  width: auto;
}

@media (max-width: 768px) {
  .custom-logo {
    max-width: 300px;
  }
}

@media (max-width: 480px) {
  .custom-logo {
    max-width: 250px;
  }
}
</style>