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
  padding: 2vh 4vw;
  display: flex;
  justify-content: space-between;
  gap: 3vw;

  .newsletter {
    display: flex;
    flex-direction: column;
    min-width: 20vw;
    max-width: 30vw;

    h5 {
      font-size: 1.5vw;
      margin-bottom: 1vw;
    }

    input {
      width: 100%;
      padding: 0.9vw;
      border-radius: 5px;
      border: none;
      background: #f3f3f3;
      margin-bottom: 1vw;
      font-size: 0.9vw;
    }

    button {
      padding: 0.8vw 0;
      border: none;
      border-radius: 6px;
      background-color: #e1306c;
      color: white;
      font-weight: 600;
      cursor: pointer;
    }
  }

  .infos {
    display: flex;
    justify-content: flex-start;
    gap: 4vw;

    article {
      display: flex;
      flex-direction: column;
      gap: 0.4vw;

      h5 {
        font-size: 1.5vw;
        margin-bottom: 0.5vw;;
      }

      a,
      p {
        font-size: 0.9vw;
        text-decoration: none;
        color: black;
      }
    }

  
  }
}

@media (max-width: 768px) {
  footer {
    flex-direction: column;
    align-items: center;
    text-align: center;

    .newsletter {
      max-width: 90%;
      width: 100%;

      h5 {
        font-size: 5vw;
      }

      input {
        height: 4vh;
        width: 90%;
        align-self: center;
        font-size: 3vw;
        text-align: center;
      }

      button {
        width: 90%;
        height: 4vh;
        margin: 0 auto;
        font-size: 3vw;
      }
    }

    .infos {
      flex-direction: column-reverse;
      gap: 3vw;
      margin-top: 2vw;
      width: 100%;

      article {
        width: 100%;
        h5 {
          font-size: 5vw;
          margin-bottom: 1vw;
        }

        a,
        p {
          font-size: 4vw;
        }
      }
    }
  }
}
</style>
