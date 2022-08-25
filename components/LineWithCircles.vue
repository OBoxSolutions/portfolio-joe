<template>
  <div>
    <div class="circle bg-text-button" />
    <div class="circle bg-text-button" />
    <div class="circle bg-text-button" />
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.circle {
  position: relative;
  border-radius: 100%;
  width: 3.125em;
  padding: 1.25em 0;
  line-height: 50px;
  text-align: center;
  margin-top: 12.5rem;
  background-color: #fff;
  z-index: 2;

  &::before{
    position: absolute;
    width: .1px;
    background-color: var(--text-color-primary);
    height: 12.5em;
    display: block;
    content: '';
    left: 50%;
    z-index: 1;
    top: -12.5em;
    margin-left: -1px;
  }
  &:first-child{
    margin-top: 0;
  }
  &:first-child::before{
    height: 1.875em;
    top: -2em;
  }
  &:last-child::after{
    position: absolute;
    width: .1px;
    background-color: var(--text-color-primary);
    height: 1.875em;
    display: block;
    content: '';
    left: 50%;
    z-index: 1;
    bottom: -1.875em;
    margin-left: -1px;
  }
}
</style>
