<script setup>

</script>


<template>
    <footer>
    <section class="infos">
    <div>
        <article>
            <h5>Contato</h5>
            <a href="mailto:contato@inspiralens.com">contato@inspiralens.com</a>
            <a href="">Central de ajuda</a>
            <p>Rio de Janeiro - Brasil</p>
        </article>
        <article>
            <h5>Sobre</h5>
            <a href="">Políticas</a>
            <a href="">Privacidade</a>
            <a href="">Blog</a>
        </article>
    </div>
        <article>
            <h5>Assine nossa newsletter</h5>
            <input type="text" id="newsletter" name="newsletter" placeholder="Seu melhor e-mail" required>
            <button type="submit">Submit</button>
        </article>
    </section>

    <section class="redes">

    </section>
</footer>
</template>


<style scoped lang="scss">
footer {
  display: flex;
  justify-content: space-between;
  margin: 2rem;
  text-align: center;  

    .infos {
        display: flex;
        flex-direction: column-reverse;
        justify-content: center;

        h5 {
            font-size: 5vw;
        }

        p {
            font-size: 4vw;
        }

        a {
            font-size: 4vw;
        }
    }

    article {
        display: flex;
        flex-direction: column;
        align-content: center;
        padding: 1vh 0;
    }
}
</style>