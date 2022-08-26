<template>
  <div id="contact" class="bg-primary">
    <h1>Contact Me</h1>
    <div class="social-networks">
      <div class="rounded-circle bg-text-button">
        <a href="#">
          <span class="icon">
            <i class="fa fa-linkedin" />
          </span>
        </a>
      </div>
      <div class="rounded-circle bg-text-button">
        <a href="#">
          <span class="icon">
            <i class="fa fa-github" />
          </span>
        </a>
      </div>
      <div class="rounded-circle bg-text-button">
        <a href="#">
          <span class="icon">
            <i class="fa fa-at" />
          </span>
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
    padding: 2px 10px;

    .icon{
      font-size: 2.2em;
      margin: auto;
      color: var(--bg-color-primary);

      &:hover{
        color: #ffffff;
      }
    }
  }
}
</style>
