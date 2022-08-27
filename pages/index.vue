<template>
  <div>
    <the-navbar />
    <div class="sections-container bg-primary">
      <section-hero />
      <section-about />
      <section-projects />
      <section-contact />
    </div>
  </div>
</template>

<script>
import SectionAbout from '~/components/SectionAbout.vue'
import SectionContact from '~/components/SectionContact.vue'
import SectionHero from '~/components/SectionHero.vue'
import SectionProjects from '~/components/SectionProjects.vue'
import TheNavbar from '~/components/TheNavbar.vue'
export default {
  name: 'IndexPage',
  components: { SectionHero, SectionAbout, SectionProjects, SectionContact, TheNavbar }
}
</script>

<style lang="scss" scoped>
.sections-container{
  display: flex;
  flex-direction: column;
  gap: 7rem;
}
</style>
