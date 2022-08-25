<template>
  <div id="projects" class="bg-primary">
    <h1>Projects</h1>
    <div class="projects-container">
      <div class="card bg-secondary" style="width: 18rem;">
        <img class="card-img-top" src="https://via.placeholder.com/400" alt="Card image cap">
        <div class="card-body">
          <h5 class="card-title color-primary">
            Card title
          </h5>
          <p class="card-text">
            Some quick example text to build on the card title and make up the bulk of the card's content.
          </p>
          <base-button class="card-button">
            Visit
          </base-button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BaseButton from './BaseButton.vue'
export default {
  name: 'SectionProjects',
  components: { BaseButton }
}
</script>

<style lang="scss" scoped>
#projects{
  .card-button{
    float: right;
  }
  .projects-container{
    display: flex;
  }
}
</style>
