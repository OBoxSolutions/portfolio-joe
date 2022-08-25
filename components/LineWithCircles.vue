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
  width: 2.4em;
  padding: 1.3em 0;
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
    height: 2.8125rem;
    top: -2.8125rem;
  }
  &:last-child::after{
    position: absolute;
    width: .1px;
    background-color: var(--text-color-primary);
    height: 2.8125rem;
    display: block;
    content: '';
    left: 50%;
    z-index: 1;
    bottom: -2.8125rem;
    margin-left: -1px;
  }
}
</style>
