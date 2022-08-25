<template>
  <div id="about" class="bg-primary color-primary">
    <div class="about-left-panel">
      <div class="about-description">
        <h1>About me</h1>
        <p>Well, the way they make shows is, they make one show. That show's called a pilot. Then they show that show to the people who make shows, and on the strength of that one show they decide if they're going to make more shows. Some pilots get picked and become television programs. Some don't, become nothing. She starred in one of the ones that became nothing.</p>
      </div>
    </div>
    <div class="about-right-panel bg-secondary">
      <h1>Skills</h1>
      <div class="right-panel-container">
        <line-with-circles class="line" />
        <div class="skills" />
      </div>
    </div>
  </div>
</template>

<script>
import LineWithCircles from './LineWithCircles.vue'
export default {
  name: 'SectionAbout',
  components: { LineWithCircles }
}
</script>

<style lang="scss" scoped>
#about{
  height: 900px;
  display: flex;

  .about-left-panel{
    width: 33.333%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .about-description{
      width: 75%;
      p{
        margin: 0;
        font-family: 'Open Sans';
        line-height: 27px;
        text-align: left;
      }
    }
  }
  .about-right-panel{
    width: 66.66%;

    h1{
      margin-top: 5rem;
      margin-left: 4rem;
    }

    .right-panel-container{
      display: flex;

      .line{
        margin-top: 7rem;
        margin-left: 4rem;
      }
    }

  }

}
</style>
