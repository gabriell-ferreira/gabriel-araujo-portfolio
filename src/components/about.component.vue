<template>
  <div class="about">
    <div class="about-desc">
      <span>Desenvolvedor front-end</span>
      <h1>Gabriel Araújo</h1>
      <p>
        Apaixonado em desenvolver soluções utilizando programação e sempre em busca de aprender coisas novas.
      </p>
    </div>
    <div class="programmer">
      <img src="../assets/Programmer.svg" alt="">
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  .about {
    margin-top: 7rem;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .about-desc {
    margin-right: 20rem;
  }
  .about-desc span {
    color: var(--blue-base);
    font-size: 2rem;
  }
  .about-desc h1 {
    font-size: 4rem;
    margin: 16px 0;
  }
  .about-desc p {
    font-size: 2rem;
    max-width: 54rem;
    line-height: 3rem;
  }

  .programmer img {
    width: 100%
  }

  @media (max-width: 1270px){
    .about-desc {
      margin: 0
    }
  }

  @media (max-width: 1000px) {
    .about {
      flex-direction: column-reverse;
    }
  }

  @media (max-width: 900px){
    .about-desc {
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .about-desc p {
      text-align: center;
    }
  }

  @media (max-width: 500px) {
    .about h1 {
      font-size: 3rem;
    }
  }



</style>