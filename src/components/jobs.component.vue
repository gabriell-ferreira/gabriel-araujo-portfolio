<template>
  <div id="jobs">
    <SectionTitle title='Trabalhos'/>
    <div class="jobs-container">
      <Job title="Happy" url='https://ik.imagekit.io/xc7bzbnt53/Home_bNdmCEkbO.png?updatedAt=1603648157656'>
        <p>
          O Happy é uma aplicação que conecta pessoas à casas de acolhimento institucional para fazer o dia de muitas crianças mais feliz.
        </p>
        <span slot="tech">Node</span>
        <span slot="tech">React</span>
        <span slot="tech">Expo</span>
        <span slot="tech">Typescript</span>

        <!-- <Button slot="app" url="#" title="Acessar"/> -->
        <Button slot='github' url="https://github.com/gabriell-ferreira/Happy-NLW" title="Github"/>
      </Job>
      <Job title="Task List" url='https://ik.imagekit.io/xc7bzbnt53/Screenshot_20210819_145748_itzWZxWoe.jpg?updatedAt=1629399801942'>
        <p>
          Gerenciador de tarefas desenvolvido para colocar em prática meus estudos com VueJs.
        </p>
        <span slot="tech">Vue</span>
        <span slot="tech">Html</span>
        <span slot="tech">Css</span>
        <span slot="tech">Javascript</span>

        <Button slot="app" url="https://task-list-jet.vercel.app/" title="Acessar"/>
        <Button slot='github' url="https://github.com/gabriell-ferreira/TaskList" title="Github"/>
      </Job><Job title="ABQAO" url='https://ik.imagekit.io/xc7bzbnt53/abq_sjdqU5Tkc.jpg?updatedAt=1630705650250'>
        <p>
          Site desenvolvido para a Associação Brasileira de Química da Amazônia Ocidental
        </p>
        <span slot="tech">Node</span>
        <span slot="tech">Vue</span>
        <span slot="tech">MongoDB</span>
        <span slot="tech">JWT token</span>

        <Button slot="app" url="https://abqamazonia.com.br/home" title="Acessar"/>
        <Button slot='github' url="https://github.com/gabriell-ferreira/abqao" title="Github"/>
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