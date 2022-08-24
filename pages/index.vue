<template>
  <div>
    <section-hero />
    <section-about />
    <section-projects />
    <section-contact />
  </div>
</template>

<script>
import SectionAbout from '~/components/SectionAbout.vue'
import SectionContact from '~/components/SectionContact.vue'
import SectionHero from '~/components/SectionHero.vue'
import SectionProjects from '~/components/SectionProjects.vue'
export default {
  name: 'IndexPage',
  components: { SectionHero, SectionAbout, SectionProjects, SectionContact }
}
</script>
