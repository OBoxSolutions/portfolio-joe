<template>
  <div id="about" class="bg-primary color-primary">
    <div class="about-left-panel">
      <div class="about-description">
        <h1>About me</h1>
        <p>Well, the way they make shows is, they make one show. That show's called a pilot. Then they show that show to the people who make shows, and on the strength of that one show they decide if they're going to make more shows. Some pilots get picked and become television programs. Some don't, become nothing. She starred in one of the ones that became nothing.</p>
      </div>
    </div>
    <div class="about-right-panel bg-secondary">
      <h1 class="panel-title">
        Skills
      </h1>
      <div class="right-panel-container">
        <line-with-circles class="line" />
        <div class="skills-container">
          <div class="skill-row">
            <div class="img-container">
              <span class="icon">
                <i class="fa fa-server" />
              </span>
            </div>
            <div class="skill-text">
              <h1 class="skill-title">
                Backend tech
              </h1>
              <p>Well, the way they make shows is, they make one show. That show's called a pilot. Then they show that show to the people who make shows, and on the strength of that one show they decide if they're going to make more shows. Some pilots get picked and become television programs. Some don't, become nothing. She starred in one of the ones that became nothing.</p>
            </div>
          </div>
          <div class="skill-row">
            <div class="img-container">
              <span class="icon">
                <i class="fa fa-database" />
              </span>
            </div>
            <div class="skill-text">
              <h1 class="skill-title">
                Databases
              </h1>
              <p>Well, the way they make shows is, they make one show. That show's called a pilot. Then they show that show to the people who make shows, and on the strength of that one show they decide if they're going to make more shows. Some pilots get picked and become television programs. Some don't, become nothing. She starred in one of the ones that became nothing.</p>
            </div>
          </div>
          <div class="skill-row">
            <div class="img-container">
              <span class="icon">
                <i class="fa fa-code" />
              </span>
            </div>
            <div class="skill-text">
              <h1 class="skill-title">
                Frontend tech
              </h1>
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

    .panel-title{
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

          .skill-title{
            font-size: 30px;
            margin: 0;
          }

          &:first-child, &:last-child{
            margin-top: 2rem;
          }
          &:last-child{
            margin-top: 1rem;
          }

          .skill-text{
            width: 70%;
            margin-left: 1.5rem;
          }
        }
      }
    }
  }

}
@media only screen and (max-width: 1400px) {
  .skill-row:last-child{
    margin-top: 0 !important;
  }
}
@media only screen and (max-width: 1285px) {
  .skills-container{
    margin-left: 1rem !important;
  }
  .line{
    margin-left: 1rem !important;
  }
  .skill-text{
    width: 90% !important;
    margin-left: 2.5rem !important;
  }
}

@media only screen and (max-width: 800px) {
  #about{
    flex-direction: column;
  }
  .about-left-panel, .about-right-panel{
    width: unset !important;
  }
  .about-description{
    width: 90% !important;
    margin-bottom: 1rem;
  }
  .panel-title{
    margin: 1rem 0 0 2rem !important;
  }
  .skills-container{
    margin-left: -1em !important;

    .skill-text{
      margin-right: 20px !important;
    }
  }
  .img-container{
    display: none;
  }
}
</style>
