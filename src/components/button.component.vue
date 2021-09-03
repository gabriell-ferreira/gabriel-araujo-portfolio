<template>
  <a id="btn" target="_blank" :href="url">{{title}}</a>
</template>

<script>
export default {
  props: ['url', 'title']
}
</script>

<style scoped>
  a {
    text-decoration: none;
    color: var(--white);
    border-radius: 13px;
    border: 3px solid var(--blue-base);
    font-size: 2rem;
    padding: 1rem 2rem;
    transition: .5s all ease;
    background-color: var(--blue-base);
  }

  a:hover {
    color: var(--black-bg);
  }
</style>