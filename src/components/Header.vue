<script setup>
import { Icon } from "@iconify/vue";
</script>


<template>
  <header>
    <img src="../assets/header/logo.svg" alt="Logo" />
    <nav>
      <ul>
        <li>
          <a href="">
            <Icon icon="material-symbols:search" width="24" height="24" />
          </a>
        </li>
        <li><a href="">inicio</a></li>
        <li><a href="">Galeria</a></li>
        <li><a href="">Favoritos</a></li>
        <li><a href=""><Icon icon="material-symbols:person" width="24" height="24" /></a></li>
      </ul>
    </nav>
  </header>
</template>


<style scoped lang="scss">
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 2rem;
  max-width: 100%;
  gap: 1rem;

  img {
    width: 2.5vw;
  }

  nav ul {
    display: flex;
    align-items: center;
    gap: 1.5rem;
    list-style: none;
    text-transform: uppercase;
  }

  a {
    text-decoration: none;
    color: black;
    font-size: 0.9rem;
  }
}

/* MOBILE */
@media (max-width: 768px) {
  header {
    flex-direction: column;
    text-align: center;

    img {
      width: 10vw;
    }

    nav ul {
      gap: 1rem;
      flex-wrap: wrap;
      justify-content: center;
    }
  }
}
</style>
