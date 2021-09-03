<template>
  <div class="title">
    <img src="../assets/Icon.svg" alt="Icon">
    <h1>{{title}}</h1>
  </div>
</template>

<script>
export default {
  props: ['title']
}
</script>

<style scoped>
  .title {
    display: flex;
    align-items: center;
    margin-bottom: 3rem;
    margin-top: 5rem;
  }
  .title h1 {
    font-size: 4rem;
    margin-left: 1rem;
  }
</style>