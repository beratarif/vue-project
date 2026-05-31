<script>
export default {
  name: 'LinkList'
}
</script>


<template>
  <ul class="nav-list">
    <li class="nav-items">
      <a class="nav-links" href="#about">Hakkımda</a>
    </li>
    <li class="nav-items">
      <a class="nav-links" href="#projects">Projelerim</a>
    </li>
    <li class="nav-items">
      <a class="nav-links" href="#contact">İletişim</a>
    </li>
  </ul>
</template>

<style>
.nav-list {
  display: flex;
  list-style: none;
  gap: 20px;
}

.nav-links {
  text-decoration: none;
  color: grey;
  transition: color 0.2s ease;
  font-size: 20px;
  font-weight: bolder;
}

.nav-links:hover {
  color: white;
}
</style>
