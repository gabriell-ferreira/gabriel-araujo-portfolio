<template>
  <div id="skills">
    <SectionTitle title='Skills'/>
    <div class="skills-container">
      <Skill technology="HTML" :path="require('../assets/Html.svg')"/>
      <Skill technology="CSS" :path="require('../assets/Css.svg')"/>
      <Skill technology="JAVASCRIPT" :path="require('../assets/Javascript.svg')"/>
      <Skill technology="VUE" :path="require('../assets/Vue.svg')"/>
    </div>
  </div>
</template>

<script>
import SectionTitle from './sectionTitle.component.vue'
import Skill from './skill.component.vue'
export default {
  components: {
    SectionTitle, Skill
  }
}
</script>

<style scoped>
  #skills {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .skills-container {
    display: flex;
    margin-top: 5rem;
  }

  .title {
    margin-top: 5rem
  }

  .skills-container #skill {
    margin: 0 6rem
  }

  @media (max-width: 900px){
    .skills-container {
      flex-direction: column;
    }

    .skills-container #skill {
      margin: 3rem 0
    }
  }
</style>