<template>
  <div class="menu">
    <div class="logo">
      <img src="../assets/Logo.svg" alt="Gabriel Araujo">
    </div>
    <nav class="menu-desktop">
      <ul>
        <li>
          <a href="#overview">Sobre</a>
        </li>
        <li>
          <a href="#">Skills</a>
        </li>
        <li>
          <a href="#">Trabalhos</a>
        </li>
        <li>
          <a href="#">Contato</a>
        </li>
      </ul>
    </nav>
    <nav class="menu-mobile">
      <img @click="handleMenu" src="../assets/Menu.svg" alt="">
      <ul v-show="menuState" :class="menuClass">
        <li>
          <a href="#overview">Sobre</a>
        </li>
        <li>
          <a href="#">Skills</a>
        </li>
        <li>
          <a href="#">Trabalhos</a>
        </li>
        <li>
          <a href="#">Contato</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>

export default {
  data(){
    return {
      menuState: false,
      menuClass: 'menu-mobile close'
    }
  },
  methods: {
    handleMenu(){
      this.menuState = !this.menuState

      this.menuState 
        ? this.menuClass = 'menu-mobile open'
        : this.menuClass = 'menu-mobile close'
    }
  }

}
</script>

<style scoped>
  .menu {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .menu-desktop ul {
    display: flex;
    list-style: none;
  }

  .menu-desktop ul li:not(:last-child) {
    margin-right: 70px;
  }

  .menu-desktop a {
    text-decoration: none;
    color: var(--dark-gray);
    font-size: 2rem;
  }

  .menu-desktop a:hover {
    color: var(--white);
    border-bottom: 3px solid var(--blue-base);
  }

  .menu-mobile {
    display: none;
  }

  .menu-mobile.open {
    position: absolute;
    list-style: none;
    background-color: var(--black-bg);
    right: 0;
    width: 50%;
    height: 100vh;
  }
  .menu-mobile.close {
    display: none;
  }

  .menu-mobile ul li {
    margin: 2rem;
    
  }

  .menu-mobile a {
    text-decoration: none;
    color: var(--white);
    font-size: 2.5rem;
  }

  @media (max-width: 1000px){
    .menu-desktop {
      display: none;
    }
    .menu-mobile {
      display: block;
    }
  }

  @media (max-width: 500px){
    .logo img {
      width: 20rem;
    }
  }

  @media (max-width: 300px){
    .logo img {
      width: 15rem;
    }
  }

</style>