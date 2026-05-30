<script setup>
import { RouterLink, RouterView } from 'vue-router';
import Navbar from './components/Navbar.vue';
import HelloWorld from './components/HelloWorld.vue';
</script>

<template>
  <Navbar/>
  <HelloWorld/>
  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  border-radius: 50%;
}

</style>
