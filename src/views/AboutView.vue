<script setup>
import { ref } from 'vue'

// Bileşen içindeki dinamik veriler
const description = ref('Merhaba! Ben Berat Arif G., tutkulu bir frontend geliştiricisiyim. Web teknolojilerine olan ilgim ve sürekli öğrenme isteğimle, kullanıcı dostu ve etkileyici web deneyimleri yaratmayı hedefliyorum. HTML, CSS, JavaScript gibi temel web teknolojilerinde güçlü bir altyapıya sahibim ve Vue.js gibi modern frameworklerle projeler geliştiriyorum. Yaratıcı çözümler bulmak ve her projede kendimi geliştirmek benim için çok önemli. İletişime geçmekten çekinmeyin, birlikte harika şeyler yapabiliriz!')

// Yetenek listesi (Buraya kolayca yeni yetenekler ekleyebilirsiniz)
const abilities = ref([
  'HTML, CSS, JavaScript',
  'Vue.js, Next.js, Bootstrap',
  'Git, GitHub',
  'Responsive Design',
  'Problem Solving',
  'Resend, Next.js API'
])
</script>

<template>
  <section id="about" class="about-section">
    <div class="container">
      <div class="about-content">
        <div class="about-image">
          <img src="../assets/profile.webp" alt="Berat Arif G. - Profil Resmi" loading="lazy">
        </div>

        <div class="about-text">
          <h1>Hakkımda</h1>
          <p>{{ description }}</p>

          <div class="about-abilities">
            <h2>Yetenekler</h2>
            <ul class="abilities-list">
              <li v-for="(ability, index) in abilities" :key="index">
                {{ ability }}
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.about-section {
  padding: 60px 0;
  background-color: #181818;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.about-content {
  display: flex;
  gap: 40px;
  align-items: center;
  flex-wrap: wrap;
  /* Mobil cihazlarda alt alta gelmesi için */
}

.about-image {
  flex: 1;
  min-width: 280px;
  text-align: center;
}

.about-image img {
  max-width: 100%;
  height: auto;
  border-radius: 50%;
  /* Yuvarlak profil resmi için */
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
}

.about-text {
  flex: 2;
  min-width: 300px;
}

.about-text h1 {
  font-size: 2.5rem;
  color: #07fb0f;
  margin-bottom: 10px;
}

.about-text h3 {
  font-size: 1.5rem;
  color: #7f8c8d;
  margin-bottom: 15px;
}

.about-text p {
  line-height: 1.6;
  color: #858585;
  margin-bottom: 25px;
}

.about-abilities h2 {
  font-size: 1.8rem;
  color: #2bff8b;
  margin-bottom: 15px;
}

.abilities-list {
  list-style: none;
  padding: 0;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 10px;
}

.abilities-list li {
  background: #000000;
  padding: 10px 15px;
  border-radius: 6px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
  border-left: 4px solid #42b983;
  /* Vue yeşili şık bir detay */
  font-weight: 500;
  color: #cdd6df;
}

/* Mobil Ekranlar İçin Ufak Ayar */
@media (max-width: 768px) {
  .about-content {
    flex-direction: column;
    text-align: center;
  }

  .abilities-list {
    text-align: left;
  }
}
</style>
