<script setup>
import 'primeicons/primeicons.css';
</script>

<template>
  <section id="contact" class="contact-section">
    <div class="container">
      <h1>İletişim</h1>
      <p>Berat Arif G. ile iletişime geçmek için aşağıdaki bilgileri kullanabilirsiniz:</p> <br>
      <ul class="contact-info">
        <li><i class="pi pi-envelope"> :</i>
          <a href="mailto:gonulberat1@gmail.com"> gonulberat1@gmail.com</a>
        </li>
        <li><i class="pi pi-phone"> :</i>
          <a href="tel:+905451724552"> +90 545 172 45 52</a>
        </li>
        <li><i class="pi pi-github"> :</i>
          <a href="https://github.com/beratarif" target="_blank"> GitHub profilim.</a>
        </li>
        <li><i class="pi pi-instagram"> :</i>
          <a href="https://www.instagram.com/berat.arif.g/" target="_blank"> Instagram adresim.</a>
        </li>
      </ul>
    </div>
  </section>
</template>

<style>
.contact-section {
  padding: 60px 0;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.contact-info {
  list-style: none;
  padding: 0;
}

.contact-info li {
  margin-bottom: 15px;
  font-size: 18px;
}

.contact-info a {
  color: #0fd167;
  text-decoration: none;
  transition: color 0.2s ease;
}

.contact-info a:hover {
  color: #0b9c4a;
}
</style>
