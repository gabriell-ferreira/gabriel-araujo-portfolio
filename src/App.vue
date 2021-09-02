<template>
  <div id="app">
    <Menu />
    <About />
    <Overview />
    <Skills />
  </div>
</template>

<script>
import Menu from './components/menu.component.vue'
import About from './components/about.component.vue'
import Overview from './components/overview.component.vue'
import Skills from './components/skills.component.vue'

export default {
  name: 'App',
  components: {
    Menu, About, Overview, Skills
  }
}
</script>

<style>
 #app {
   padding: 72px;
   color: var(--white);
   height: 100vh;
 }

 @media (max-width: 700px) {
    #app {
      padding:50px 20px;
    }
  }
</style>
