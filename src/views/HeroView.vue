<template>
  <section id="hero" class="container">
    <div class="hero-section">
      <div class="hero-content">
        <div class="hero-links">
          <h1>Merhaba, Ben <span class="green">Berat Arif G</span></h1>
          <h3>Frontend Developer</h3>
        </div>
        <div class="hero-profile">
          <img src="../assets/profile.webp" alt="Profile Picture">
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
  flex-direction: column;
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
.hero-profile img{
  width:500px;
  height: 500px;
  border-radius: 50%;
  align-items: center;
  text-align: center;
}

.green{
  animation: fadeIn 1s ease-in-out;
  font-size: 50px;
  font-weight: 800;
  color: #0fd167;
}

.green:hover{
  color: #0fd167;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

</style>
