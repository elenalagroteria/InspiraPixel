<script setup>
defineProps(["imagem"]);
import { Icon } from "@iconify/vue";

import { ref } from "vue";

const deuLike = ref(false);

const alternarCor = () => {
  deuLike.value = !deuLike.value;
};

</script>

<template>
  <div class="card">
    <button
      class="iconePadrao"
      :class="{ clicou: deuLike }"
      @click="alternarCor"><Icon icon="material-symbols:heart-smile-rounded" width="24" height="24"/></button>
    <img
      :src="imagem"
      alt="Imagens"
    />
  </div>
</template>

<style scoped lang="scss">
.card {
  width: 30vw;
  min-width: 260px;
  height: 45vh;
  position: relative;
  display: flex;

  img {
    border-radius: 10px;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  button {
    position: absolute;
    right: 10px;
    top: 10px;
    background-color: transparent;
    border: none;
    filter: drop-shadow(0px 2px 40px black);
  }
  }

.iconePadrao :deep(svg) {
  color: #ffffff;
  }

.clicou :deep(svg) {
  color: #F93838;
}

</style>
