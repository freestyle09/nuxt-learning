<template>
  <button
    class="button"
    v-bind="$attrs"
    :class="isRed ? 'red' : 'blue'"
    v-on="$listeners"
    @click="$emit('onClick')"
  >
    <slot />
  </button>
</template>

<script>
export default {
  props: {
    isRed: {
      type: Boolean
    }
  },
  mounted () {
    console.log(this.isRed)
  }
}
</script>

<style scoped>
.button {
  padding: 0.3rem 1rem;
  transition: 0.2s ease;
  cursor: pointer;
}
.red {
  background-color: red;
  color: rgba(0, 0, 0, 0.8);
}
.blue {
  background-color: blue;
  color: #fff;
}
</style>
