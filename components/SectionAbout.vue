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
        <div class="skills-container">
          <div class="skill-row">
            <div class="img-container">
              <!-- <img src="/backend.svg" alt="backend"> -->
              <span class="icon">
                <i class="fa fa-server" />
              </span>
            </div>
            <div class="skill-text">
              <h1>Backend tech</h1>
              <p>Well, the way they make shows is, they make one show. That show's called a pilot. Then they show that show to the people who make shows, and on the strength of that one show they decide if they're going to make more shows. Some pilots get picked and become television programs. Some don't, become nothing. She starred in one of the ones that became nothing.</p>
            </div>
          </div>
          <div class="skill-row">
            <div class="img-container">
              <!-- <img src="/databases.svg" alt="databases"> -->
              <span class="icon">
                <i class="fa fa-database" />
              </span>
            </div>
            <div class="skill-text">
              <h1>Databases</h1>
              <p>Well, the way they make shows is, they make one show. That show's called a pilot. Then they show that show to the people who make shows, and on the strength of that one show they decide if they're going to make more shows. Some pilots get picked and become television programs. Some don't, become nothing. She starred in one of the ones that became nothing.</p>
            </div>
          </div>
          <div class="skill-row">
            <div class="img-container">
              <!-- <img src="/frontend.svg" alt="frontend"> -->
              <span class="icon">
                <i class="fa fa-code" />
              </span>
            </div>
            <div class="skill-text">
              <h1>Frontend tech</h1>
              <p>Well, the way they make shows is, they make one show. That show's called a pilot. Then they show that show to the people who make shows, and on the strength of that one show they decide if they're going to make more shows. Some pilots get picked and become television programs. Some don't, become nothing. She starred in one of the ones that became nothing.</p>
            </div>
          </div>
        </div>
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
  // height: 900px;
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
    margin-bottom: 2rem;

    h1{
      margin: 5rem 0 2rem 4rem;
    }

    .right-panel-container{
      display: flex;
      margin-bottom: 4rem;

      .line{
        margin-top: 7rem;
        margin-left: 4rem;
      }

      .skills-container{
        margin-top: 1rem;
        margin-left: 2rem;
        display: flex;
        flex-direction: column;
        gap: 3.5rem;

        .img-container{
          width: 15%;
          .icon{
            font-size: 7em;
            color: var(--text-color-primary);
          }
        }

        .skill-row{
          display: flex;

          h1{
            font-size: 30px;
          }

          &:first-child{
            margin-top: 2rem;
          }
          &:last-child{
            margin-top: 2rem;
          }

          .skill-text{
            width: 70%;
            margin-left: 1.5rem;

            h1, p{
              margin: 0;
            }
          }
        }
      }
    }

  }

}
</style>
