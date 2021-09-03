<template>
  <div id="app">
    <Menu />
    <About />
    <Overview />
    <Skills />
    <Jobs />
    <Contact />

    <footer>
      <span>&copy; 2021 - Gabriel Araújo Ferreira</span>
    </footer>
  </div>
</template>

<script>
import Menu from './components/menu.component.vue'
import About from './components/about.component.vue'
import Overview from './components/overview.component.vue'
import Skills from './components/skills.component.vue'
import Jobs from './components/jobs.component.vue'
import Contact from './components/contact.component.vue'

export default {
  name: 'App',
  components: {
    Menu, About, Overview, Skills, Jobs, Contact
  }
}
</script>

<style>
 #app {
   padding: 72px;
   color: var(--white);
   height: 100vh;
 }

 footer {
   font-size: 2rem;
   color: var(--dark-gray);
   display: flex;
   justify-content: center;
   margin: 5rem;
 }

 footer span {
   margin-bottom: 1rem;
   text-align: center;
 }

 @media (max-width: 900px) {
   footer {
     font-size: 1rem;
   }
 }

 @media (max-width: 700px) {
    #app {
      padding:50px 20px;
    }
  }
</style>
