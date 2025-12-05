<script setup>
defineProps(["imagem"]);
</script>

<template>
  <div class="card">
    <button>💖</button>
    <img
      :src="imagem"
      alt="Praia de São Conrado"
    />
  </div>
</template>

<style scoped lang="scss">
.card {
  width: 30vw;
  height: 50vh;
  position: relative;
  
  img {
    border-radius: 10px;
    width: 100%;
    height: 100%;
  }
  
  button {
    position: absolute;
    right: 10px;
    background-color: transparent;
    border: none;
  }
}
</style>