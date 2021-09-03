<template>
  <div id="job">
    <div class="job-img">
      <img :src="url" :alt="title">
    </div>

    <h1>{{title}}</h1>
    <slot></slot>

    <div class="job-hover">
      <h1>{{title}}</h1>
      <slot></slot>
      <div class="tech-container">
        <slot name="tech"></slot>
      </div>
      <div class="buttons">
        <slot name="app"></slot>
        <slot name="github"></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jobHover: false
    }
  },
  props: ['url', 'title']
}
</script>

<style scoped>
  #job {
    max-width: 385px;
    height: 430px;
    border-radius: 13px;
    border: 7px solid var(--blue-base);
    padding: 1rem;

    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
  }

  #job h1 {
    font-size: 3rem;
    margin: 2rem 0
  }

  #job p {
    font-size: 1.5rem;
    text-align: justify;
    user-select: none;
  }

  #job span {
    font-size: 1.5rem;
    border-radius: 7px;
    border: 3px solid var(--blue-base);
    padding: 1rem 2rem;
    margin: 1rem;
  }

  #job img {
    width: 100%;
    border-radius: 13px;
  }

  #job .buttons {
    display: flex;
  }

  #btn {
    margin: 2rem 1rem
  }

  .tech-container {
    margin: 2rem 0 0 0;
    display: flex;
    justify-content: flex-start;
    flex-wrap: wrap;
  }

  .job-hover {
    background-color: #12043F;
    position: absolute;
    height: 100%;
    width: 100%;
    top:0;
    display: none;
    border-radius: 5px;
    padding: 1rem;
  }

  #job:hover .job-hover {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  @media (max-width:900px) {
    .buttons {
      flex-direction: column;
    }

    #btn {
      margin: .5rem 0
    }
  }
</style>