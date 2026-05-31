<script setup>

// Give the component a multi-word name to satisfy linting rules
defineOptions({ name: 'AppNavbar' })

import Links from './Link/Links.vue';

</script>

<template>
  <section class="navbar-section">
    <div class="container">
      <div class="navbar">
        <div class="nav-header">
          <h1> Berat Arif G</h1>
        </div>
        <Links />
      </div>
    </div>
  </section>
</template>

<style>
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px;
}

.nav-header h1 {
  display: flex;
  align-items: center;
  gap: 10px;
  font-size: 24px;
  font-weight: bold;
  color: #0fd167;
}
</style>
