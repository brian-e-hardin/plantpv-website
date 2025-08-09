<template>
  <header class="site-header">
    <div class="container">
      <div class="header-content">
        <div class="site-branding">
          <a href="#" class="custom-logo-link">
            <img 
              src="/plant-pv-logo.jpg" 
              alt="Plant PV" 
              class="custom-logo"
            />
          </a>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup lang="ts">
</script>

<style scoped>
.site-header {
  background: #fff;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  padding: 1rem 0;
}

.header-content {
  display: flex;
  align-items: center;
  justify-content: center;
}

.site-branding {
  text-align: center;
}

.custom-logo-link {
  display: inline-block;
}

.custom-logo {
  height: auto;
  max-width: 100%;
  width: auto;
  max-height: 80px;
}

@media (max-width: 768px) {
  .custom-logo {
    max-height: 60px;
  }
}
</style>