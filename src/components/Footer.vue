<script setup>

</script>


<template>
  <footer>
    <section class="newsletter">
      <h5>Assine nossa newsletter</h5>
      <input type="email" placeholder="Seu email" />
      <button>Inscrever-se</button>
    </section>

    <section class="infos">
      <article>
        <h5>Contato</h5>
        <a href="mailto:contato@inspiralens.com">contato@inspiralens.com</a>
        <a href="#">Central de ajuda</a>
        <p>Rio de Janeiro – Brasil</p>
      </article>

      <article>
        <h5>Sobre</h5>
        <a href="#">Políticas</a>
        <a href="#">Políticas de privacidade</a>
        <a href="#">Blog</a>
      </article>
    </section>
  </footer>
</template>


<style scoped lang="scss">
footer {
  width: 100%;
  padding: 3rem 2rem;
  display: flex;
  justify-content: space-between;
  gap: 3rem;

  /* Desktop — três colunas */
  .newsletter,
  .infos {
    flex: 1;
  }

  .newsletter {
    display: flex;
    flex-direction: column;
    max-width: 350px;

    h5 {
      font-size: 1.1rem;
      margin-bottom: 1rem;
    }

    input {
      width: 100%;
      padding: 0.9rem;
      border-radius: 5px;
      border: none;
      background: #f3f3f3;
      margin-bottom: 1rem;
      font-size: 0.9rem;
    }

    button {
      padding: 0.8rem 0;
      border: none;
      border-radius: 6px;
      background-color: #e1306c;
      color: white;
      font-weight: 600;
      cursor: pointer;
    }
  }

  /* Contato + Sobre (lado a lado no desktop) */
  .infos {
    display: flex;
    justify-content: flex-start;
    gap: 4rem;

    article {
      display: flex;
      flex-direction: column;
      gap: 0.4rem;

      h5 {
        font-size: 1.1rem;
        margin-bottom: 0.5rem;
      }

      a,
      p {
        font-size: 0.9rem;
        text-decoration: none;
        color: black;
      }
    }
  }
}

/* 📱 MOBILE — exatamente como a imagem que você enviou */
@media (max-width: 768px) {
  footer {
    flex-direction: column;
    align-items: center;
    text-align: center;

    .newsletter {
      max-width: 90%;
      width: 100%;

      h5 {
        font-size: 1.4rem;
      }

      button {
        width: 60%;
        margin: 0 auto;
        font-size: 1rem;
      }
    }

    .infos {
      flex-direction: column-reverse;
      gap: 3rem;
      margin-top: 2rem;
      width: 100%;

      article {
        width: 100%;
        h5 {
          font-size: 1.4rem;
          margin-bottom: 1rem;
        }

        a,
        p {
          font-size: 1.1rem;
        }
      }
    }
  }
}
</style>
