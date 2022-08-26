<template>
  <div id="projects" class="bg-primary">
    <h1>Projects</h1>
    <div class="projects-container">
      <div v-for="(project, index) in projects" :key="`project-${index}`" class="card bg-secondary" style="width: 18rem;">
        <img class="card-img-top" :src="project.image" alt="Project image cap">
        <div class="card-body">
          <h5 class="card-title color-primary">
            {{ project.title }}
          </h5>
          <p class="card-text">
            {{ project.text }}
          </p>
          <div class="card-image-overlay m-auto">
            <span v-for="(tag, indexTag) in project.tags" :key="`tag-${indexTag}`" class="card-detail-badge bg-primary">
              <small class="text-muted badge-text"> {{ tag }} </small>
            </span>
          </div>
          <base-button class="card-button">
            <a :href="project.link">Visit</a>
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
  components: { BaseButton },
  data () {
    return {
      projects: [
        { title: 'Title', text: "Well, the way they make shows is, they make one show. That show's called a pilot.", tags: ['HTML', 'CSS', 'Javascript'], image: '/projects/400x400.png', link: '#' },
        { title: 'Title', text: "Well, the way they make shows is, they make one show. That show's called a pilot.", tags: ['HTML', 'CSS', 'Javascript'], image: '/projects/400x400.png', link: '#' },
        { title: 'Title', text: "Well, the way they make shows is, they make one show. That show's called a pilot.", tags: ['HTML', 'CSS', 'Javascript'], image: '/projects/400x400.png', link: '#' },
        { title: 'Title', text: "Well, the way they make shows is, they make one show. That show's called a pilot.", tags: ['HTML', 'CSS', 'Javascript'], image: '/projects/400x400.png', link: '#' },
        { title: 'Title', text: "Well, the way they make shows is, they make one show. That show's called a pilot.", tags: ['HTML', 'CSS', 'Javascript'], image: '/projects/400x400.png', link: '#' },
        { title: 'Title', text: "Well, the way they make shows is, they make one show. That show's called a pilot.", tags: ['HTML', 'CSS', 'Javascript'], image: '/projects/400x400.png', link: '#' },
        { title: 'Title', text: "Well, the way they make shows is, they make one show. That show's called a pilot.", tags: ['HTML', 'CSS', 'Javascript'], image: '/projects/400x400.png', link: '#' },
        { title: 'Title', text: "Well, the way they make shows is, they make one show. That show's called a pilot.", tags: ['HTML', 'CSS', 'Javascript'], image: '/projects/400x400.png', link: '#' }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
#projects{
  h1{
    margin: 0 2rem 3rem;
  }

  h5{
    font-family: 'Amiko', sans-serif;
    font-size: 2em;
  }

  .projects-container{
    margin-left: 2.5rem;
    display: flex;
    flex-wrap: wrap;
    gap: 6rem;
    padding-bottom: 3rem;
  }
  .card{
    border: none !important;
  }
  .card-button{
    float: right;
    margin-top: 3rem;
    padding: 2px 1.5em;
    border-radius: 5px;
  }
  .card-detail-badge {
    text-align: center;
    border-radius: 30px 30px 30px 30px;
    padding: 3px 8px;
    margin: 3px;
    font-size: 14px;

    .badge-text{
      color: var(--badge-color);
    }
  }
}

@media only screen and (max-width: 400px) {
  .projects-container{
    margin-left: 0 !important;
    justify-content: center !important;
  }
}
</style>
