<template>
  <div id="home" class="bg-primary color-primary">
    <h1 class="home-title">
      Catchy phrase here
    </h1>
    <div class="home-picture">
      <img src="https://via.placeholder.com/400" alt="profile-image">
    </div>
    <div class="home-description bg-primary">
      <p>Well, the way they make shows is, they make one show. That show's called a pilot.</p>
    </div>
    <base-button class="home-button" @click.prevent="scrollToPosition('#projects')">
      My projects
    </base-button>
  </div>
</template>

<script>
import BaseButton from './BaseButton.vue'
export default {
  name: 'SectionHero',
  components: { BaseButton },
  methods: {
    scrollToPosition (postitionId) {
      const elmnt = document.getElementById(postitionId.split('#').pop())
      elmnt.scrollIntoView({ behavior: 'smooth' })
    }
  }
}
</script>

<style lang="scss" scoped>
$navbar-height: 100px;

#home{
  display: flex;
  flex-direction: column;
  align-items: center;
  height: calc(100vh - $navbar-height);

  .home-title{
    margin-bottom: 1rem;
    font-family: 'Open Sans';
    font-size: 60px;
    text-align: center;
  }

  .home-picture{
    display: flex;
    justify-content: center;
    img{
      border-radius: 50%;
      object-fit: contain;
    }
  }
  .home-description{
    width: 30%;
    margin-top: .5rem;
  }
  p{
    font-family: 'Amiko';
    font-size: 1em;
    text-align: center;
  }
}
.home-button{
  font-family: 'Amiko';
  font-size: 20px;
  line-height: 43px;
}

@media only screen and (max-width: 800px) {
  .home-picture{
    display: flex;
    justify-content: center;
    img{
      width: 95%;
    }
  }
  .home-description{
    width: 90% !important;
  }
}
</style>
