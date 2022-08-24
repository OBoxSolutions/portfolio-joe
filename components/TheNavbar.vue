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
    <div class="navbar-theme-switcher">
      <img src="/theme-switch.svg" alt="theme-switch">
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
  methods: {
    scrollToPosition (postitionId) {
      const elmnt = document.getElementById(postitionId.split('#').pop())
      elmnt.scrollIntoView({ behavior: 'smooth' })
    }
  }

}
</script>

<style lang="scss" scoped>
.navbar{
  padding: 3.5rem;
  display: flex;

  .navbar-menu{
    margin: auto;
    display: flex;
    gap: 1rem;

    .navbar-menu-item{
      list-style-type: none;
      a{
        text-decoration: none;
      }
    }
  }

  .navbar-theme-switcher{
    margin-left: auto;
    cursor: pointer;
  }
}

</style>
