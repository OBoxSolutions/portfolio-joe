<template>
  <div id="projects">
    <div class="card" style="width: 18rem;">
      <img class="card-img-top" src="https://via.placeholder.com/400" alt="Card image cap">
      <div class="card-body">
        <h5 class="card-title">
          Card title
        </h5>
        <p class="card-text">
          Some quick example text to build on the card title and make up the bulk of the card's content.
        </p>
        <base-button>Visit</base-button>
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

<style>

</style>
