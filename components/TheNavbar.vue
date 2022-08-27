<template>
  <nav class="navbar bg-primary color-primary">
    <h1 class="navbar-title">
      Joseph Cannon
    </h1>
    <ul class="navbar-menu">
      <li v-for="(link, index) in links" :key="`link-${index}`" class="navbar-menu-item">
        <a :href="link.link" class="color-primary" @click.prevent="scrollToPosition(link.link)">
          {{ link.text }}
        </a>
      </li>
    </ul>
    <div class="navbar-theme-switcher" @click="toggleTheme">
      <span class="icon">
        <i class="fa fa-adjust" />
      </span>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'TheNavbar',
  data () {
    return {
      links: [
        { text: 'About', link: '#about' },
        { text: 'Projects', link: '#projects' },
        { text: 'Contact Me', link: '#contact' }
      ]
    }
  },
  mounted () {
    if (localStorage.getItem('theme') === 'theme-light') {
      this.setTheme('theme-light')
    } else {
      this.setTheme('theme-dark')
    }
  },
  methods: {
    scrollToPosition (postitionId) {
      const elmnt = document.getElementById(postitionId.split('#').pop())
      elmnt.scrollIntoView({ behavior: 'smooth' })
    },
    toggleTheme () {
      if (localStorage.getItem('theme') === 'theme-dark') {
        this.setTheme('theme-light')
      } else {
        this.setTheme('theme-dark')
      }
    },
    setTheme (themeName) {
      localStorage.setItem('theme', themeName)
      document.documentElement.className = themeName
    }
  }

}
</script>

<style lang="scss" scoped>
$navbar-height: 100px;
.navbar{
  height: $navbar-height;
  padding: 1rem 3.5rem;
  display: flex;

  .navbar-title{
    position: absolute;
  }

  .navbar-menu{
    margin: 2rem auto;
    display: flex;
    gap: 1rem;

    .navbar-menu-item{

      list-style-type: none;
      a{
        &:hover{
          color: var(--color-link) !important;
        }
      }
    }
  }
  .navbar-theme-switcher{
    position: absolute;
    top: 1.5em;
    right: 1.5em;
    cursor: pointer;
    .icon{
      font-size: 1.5em;
    }
  }
}

@media only screen and (max-width: 800px) {
  .navbar{
    flex-direction: column;
    align-items: center;

    .navbar-menu{
      margin: auto !important;
    }
    .navbar-title{
      text-align: center;
      position: unset !important;
    }
  }
}
</style>
