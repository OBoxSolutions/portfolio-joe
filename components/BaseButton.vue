<template>
  <button
    class="button bg-text-button"
    v-bind="$attrs"
    v-on="$listeners"
  >
    <slot />
  </button>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

.button{
  color: #ffffff;
  border: none;
  outline: none;
  border-radius: 10px;
  padding: 0 1.3rem;
  cursor: pointer;

  &:hover{
    background-color: var(--color-hover-button) !important;
  }
}

</style>
