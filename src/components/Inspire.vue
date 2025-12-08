<script setup>
import { ref } from "vue";
import Card from "./Card.vue";
// Ele nos permite buscar dados de APIs externas de forma simples.
import axios from "axios";
// Criamos uma variável reativa que vai guardar a lista de imagens.
const imagens = ref([]);
async function carregarImagens() {
  const res = await axios.get("https://picsum.photos/v2/list?page=2&limit=12");

  imagens.value = res.data;

  console.log(res);
}
carregarImagens();
</script>


<template>
  <section class="inspire">
    <h2>Inspire-se</h2>
    <section class="cards">
    <Card v-for="img in imagens" :imagem="img.download_url" />
  </section>
  </section>
</template>


<style scoped lang="scss">
.inspire {
  margin: 1rem;
}

h2 {
  text-align: center;
  font-size: 8vh;
  margin-bottom: 2vh;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: center;
}

@media (max-width: 600px) {
  .cards {
    justify-content: center;
  }
}
</style>
