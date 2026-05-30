<script setup>
import Navbar from './components/Navbar.vue';
import HeroView from './views/HeroView.vue';
import AboutView from './views/AboutView.vue';
import ContactView from './views/ContactView.vue';
import FooterView from './views/FooterView.vue';
import ProjectView from './views/ProjectView.vue';
</script>

<template>
  <Navbar />
  <HeroView />
  <AboutView />
  <ProjectView />
  <ContactView />
  <FooterView />
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
