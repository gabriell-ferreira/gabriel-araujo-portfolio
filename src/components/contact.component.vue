<template>
  <div id="contact">
    <SectionTitle title="Contato"/>

    <div class="contacts-container">
      <div class="line">
        <div class="contact">
          <img src="../assets/Phone.svg" alt="">
          <span>(92) 99333-5746</span>
        </div>
        <div class="contact">
          <img src="../assets/Git.svg" alt="">
          <a target="_blank" href="https://github.com/gabriell-ferreira">gabriell-ferreira</a>
        </div>
      </div>
      <div class="line">
        <div class="contact">
          <img src="../assets/Email.svg" alt="Email">
          <a target="_blank" href="mailto:araujogabriel80@hotmail.com?subject=Olá%20podemos%20conversar?">araujogabriel80@hotmail.com</a>
        </div>
        <div class="contact">
          <img src="../assets/Linkedin.svg" alt="Linkedin">
          <a target="_blank" href="https://www.linkedin.com/in/gabriel-ferreira-7a92241a3/">Gabriel Ferreira</a>
        </div>
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

<style>
  #contact {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 5rem;
  }
  span {
    font-size: 2rem;
  }
  .contacts-container {
    width: 70%;

    display: flex;
    flex-direction: column;
  }
  .contact {
    display: flex;
    align-items: center;
  }
  .contact img {
    margin-right: 1rem;
  }
  .contact a {
    text-decoration: none;
    color: var(--white);
    font-size: 2rem;
    transition: color.5s ease;
  }
  .contact a:hover {
    color: var(--blue-base);
  }
  .line {
    margin: 5rem 0;
    display: flex;
    justify-content: space-between;
    width: 100%;
  }

  @media (max-width: 900px){
    .contacts-container {
      width: 100%
    }
    .line {
      flex-direction: column;
      margin: 1rem 0
    }
    .contact {
      flex-direction: column;
      margin: 1rem
    }
    .contact img {
      margin: 1rem;
    }
    .contact span {
      font-size: 1.900rem;
    }
    .contact a {
      font-size: 1.5rem;
    }
  }
</style>