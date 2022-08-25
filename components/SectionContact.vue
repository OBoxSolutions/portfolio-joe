<template>
  <div id="contact" class="bg-primary">
    <h1>Contact Me</h1>
    <div class="social-networks">
      <div class="rounded-circle bg-text-button">
        <a href="#">
          <img src="/linked-in.svg" alt="linked-in">
        </a>
      </div>
      <div class="rounded-circle bg-text-button">
        <a href="#">
          <img src="/github.svg" alt="github">
        </a>
      </div>
      <div class="rounded-circle bg-text-button">
        <a href="#">
          <img src="/email.svg" alt="email">
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SectionContact'
}
</script>

<style lang="scss" scoped>
#contact{
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1em;

  .social-networks{
    display: flex;
    gap: 1em;
    margin-bottom: 3rem;
  }
  .rounded-circle{
    padding: .5em;

    img{
      width: 1.5em;
    }
  }
}
</style>
