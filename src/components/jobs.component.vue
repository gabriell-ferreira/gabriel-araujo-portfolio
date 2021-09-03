<template>
  <div id="jobs">
    <SectionTitle title='Trabalhos'/>
    <div class="jobs-container">
      <Job title="Happy" url='https://ik.imagekit.io/xc7bzbnt53/Home_bNdmCEkbO.png?updatedAt=1603648157656'>
        <p>
          O Happy é uma aplicação que conecta pessoas à casas de acolhimento institucional para fazer o dia de muitas crianças mais feliz.
        </p>
        <span slot="tech">React</span>
        <span slot="tech">Html</span>
        <span slot="tech">Css</span>
        <span slot="tech">Javascript</span>

        <Button slot="app" url="#" title="Acessar"/>
        <Button slot='github' url="#" title="Github"/>
      </Job>
      
    </div>
  </div>
</template>

<script>
import SectionTitle from './sectionTitle.component.vue'
import Job from './job.component.vue'
import Button from './button.component.vue'
export default {
  components: {
    SectionTitle, Job, Button
  }
}
</script>

<style scoped>
  #jobs {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .jobs-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }

  #job {
    margin: 2rem
  }
</style>