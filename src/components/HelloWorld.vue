<script setup>

</script>

<template>
  <section class="hero-section">
    <div class="container">
      <div class="hero-content">
        <div class="hero-profile">
          <img src="../assets/IMG_20260529_202913_288.webp" alt="">
        </div>
        <div class="hero-text">
          <h1 class="green">Berat Arif G.</h1>
          <h3>Front-End Developer</h3>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.container {
  max-width: 1920px;
  width: 100%;
  margin: 0 auto;
  padding: 20px;
}

.hero-section {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100vh;
}

.hero-content{
  display:flex;
  justify-content: center;
  gap:120px;
  align-items: center;
  width: 100%;
}

.hero-links {
  display: flex;
  align-items: center;
  text-align: center;
}

h1 {
  font-size: 50px;
  font-weight: 800;
}

h3 {
  font-size: 30px;
  font-weight: 500;
  color: grey;
}

.green{
  color: #0fd167;
  font-weight: 800;

}

.hero-profile img{
  width:500px;
  height: 500px;
  border-radius: 50%;
  align-items: center;
  text-align: center;
}
</style>
