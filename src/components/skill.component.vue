<template>
  <div id="skill">
    <h1>{{technology}}</h1>
    <img :src="path" :alt="technology">
  </div>
</template>

<script>
export default {
  props: {
    technology: {
      type: String
    },
    path: {
      type: String
    }
  }
}
</script>

<style scoped>
  #skill {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
  }

  #skill h1 {
    font-size: 2rem;
    margin-bottom: 1rem;
  }
</style>