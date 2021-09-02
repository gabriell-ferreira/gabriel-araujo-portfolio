<template>
  <div id="overview">
    <div class="avatar">
      <div class="avatar-img">
        <img src="../assets/Avatar.jpg" alt="Gabriel Araujo Ferreira">
      </div>
      <div class="social-icons">
        <a target="_blank" href="mailto:araujogabriel80@hotmail.com?subject=Olá%20podemos%20conversar?">
          <img src="../assets/Email.svg" alt="Email">
        </a>
        <a target="_blank" href="https://github.com/gabriell-ferreira">
          <img src="../assets/Git.svg" alt="Github">
        </a>
        <a target="_blank" href="https://www.linkedin.com/in/gabriel-ferreira-7a92241a3/">
          <img src="../assets/Linkedin.svg" alt="Linkedin">
        </a>
      </div>
    </div>
    <div class="desc">
      <SectionTitle title='Sobre'/>
      <p>Conheça um pouco sobre mim</p>

      <div class="about-me">
        <p>
          Me chamo Gabriel, tenho 20 anos, moro em Manaus-AM, sou estudante de Ciência da Computação e a 1 ano me dedico aos estudos na área de front-end.
        </p>
        <p>
          Sempre fui fã de tecnologia e resolver problemas, a programação potencializou esse desejo e hoje estou sempre a disposição para aprender cada vez mais e desenvolver soluções.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import SectionTitle from './sectionTitle.component.vue'
export default {
  components: {
    SectionTitle
  }
}
</script>

<style scoped>
  #overview {
    height: 100vh;
    width: 100%;

    display: flex;
    justify-content: center;
    align-items: center;
  }

  .avatar {
    display: flex;
    flex-direction: column;
    align-items: center;
    flex: 1;
  }

  .avatar-img {
    width: 228px;
  }

  .avatar-img img {
    border-radius: 50%;
    border: 5px solid var(--blue-base);
    width: 100%;
  }

  .social-icons {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 2rem;
  }

  .social-icons a:nth-child(2){
    margin: 0 50px
  }

  .desc {
    flex: 1;
  }

  .desc p{
    font-size: 2rem;
  }
  .desc .about-me {
    width: 70%;
    color: var(--dark-gray);
    margin-top: 3rem;
  }
  .desc .about-me p:first-of-type {
    margin-bottom: 1rem;
  }

  @media (max-width: 900px){
    #overview {
      flex-direction: column;
      height: auto;
      margin: 20rem 0;
    }

    .avatar {
      margin: 5rem 0;
    }

    .desc {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .desc p {
      text-align: center;
    }

    .desc .about-me {
      text-align: justify;
      width: auto;
    }
  }

</style>