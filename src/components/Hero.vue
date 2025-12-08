<script setup>  </script>

<template>
    <section class="hero">
        <div>
        <h2>
            Onde a paisagem vira <span>inspiração</span>.
        </h2>
        <p>Explore paisagens, cores e luzes que inspiram novas histórias através da fotografia.</p>
        </div>

        <img src="../assets/hero/fotografo.png" alt="Imagem ilustrativa" />

    </section>


</template>

<style scoped lang="scss">
.hero {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 3rem 2rem;
  gap: 2rem;
  flex-wrap: wrap;

  h2 {
    font-size: 2.4rem;
    line-height: 1.2;

    span {
      color: #E1306C;
      font-size: 3.2rem;
    }
  }

  p {
    max-width: 400px;
    margin-top: 1rem;
  }

  img {
    width: 38vw;
    min-width: 280px;
  }
}

/* MOBILE */
@media (max-width: 768px) {
  .hero {
    text-align: center;
    justify-content: center;

    img {
      width: 80%;
    }

    h2 {
      font-size: 2rem;

      span {
        font-size: 2.4rem;
      }
    }
  }
}
</style>
