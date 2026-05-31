<script setup>
import { ref } from 'vue';

  const projects = ref([
    {
      title: 'Tailwind CSS ile Kişisel Web Sitesi',
      description: 'Bu proje, Tailwind CSS kullanarak oluşturduğum kişisel web sitemdir. Modern ve minimalist bir tasarıma sahip olan bu site, benim hakkımda bilgi verirken aynı zamanda projelerimi ve iletişim bilgilerimi de içeriyor.',
      link: 'https://beratarif.netlify.app/'
    },
    {
      title: 'Next.js ile Portfolio Sitesi',
      description: 'Bu proje, Next.js kullanarak oluşturduğum kişisel portfolio sitemdir. Modern ve responsive bir tasarıma sahip olan bu site, benim projelerimi ve becerilerimi gösterirken aynı zamanda iletişim bilgilerimi de içeriyor.',
      link: 'https://beratarif.vercel.app/'
    },
    {
      title: 'Hava Durumu Uygulaması',
      description: 'Bu, Hava Durumu Uygulaması her gün hava durumu bilgilerini sağlar. Kullanıcılar, şehir adını girerek o şehirdeki güncel hava durumunu görebilirler. Uygulama, açık hava durumunu göstermek için görseller ve simgeler kullanır.',
      link: 'https://havadurumujson.netlify.app/'
    },
    {
      title: 'Json Login',
      description: 'Bu, Json Login uygulaması kullanıcıların kimlik doğrulaması yapmalarına olanak tanır.',
      link: 'https://jsonlogin.netlify.app/'
    },
    {
      title: 'Json Notepad',
      description: 'Bu, Json Notepad uygulaması kullanıcıların notlarını kaydetmelerine ve yönetmelerine olanak tanır.',
      link: 'https://notdefterijson.netlify.app/'
    },
    {
      title: 'CodeProo - Kod Paylaşım Platformu',
      description: 'Bu, CodeProo - Kod Paylaşım Platformu kullanıcıların temel kodlama bilgilerini paylaşmalarına ve öğrenmelerine olanak tanır.',
      link: 'https://codeproo.netlify.app/'
    }

  ]);
</script>

<template>
  <section id="projects" class="project-section">
    <div class="container">
      <h1>Projeler</h1>
      <p>Aşağıda yer alan projelerimi inceleyebilirsiniz:</p>
      <div class="projects-list">
        <div v-for="(project, index) in projects" :key="index" class="project-item">
          <h2>{{ project.title }}</h2>
          <p>{{ project.description }}</p>
          <a :href="project.link" target="_blank">Projeyi Görüntüle</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.project-section {
  padding: 40px 0;
}
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}
.projects-list {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 20px;

}
.project-item {
  background-color: #303030;
  padding: 20px;
  border-radius: 8px;
  flex: 1 1 calc(33.333% - 40px);
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}
.project-item h2 {
  font-size: 1.5rem;
  margin-bottom: 10px;
  color: #0fd167;
}
.project-item p {
  font-size: 1rem;
  margin-bottom: 15px;
  color: #cdd6df;
}
.project-item a {
  color: #0fd167;
  text-decoration: none;
  font-weight: 500;
  transition: color 0.2s ease;
}
.project-item a:hover {
  color: #0b9c4a;
}
</style>
