<template>
  <Button :is-red="isRed" @onClick="handleButtonClick">
    Kliknij mnie :) !
  </Button>
</template>
<script>
import Button from '../Button'

export default {
  components: {
    Button
  },
  data () {
    return {
      isRed: true
    }
  },
  methods: {
    handleButtonClick (msg) {
      this.isRed = !msg
    }
  }
}
</script>

<style scoped></style>
