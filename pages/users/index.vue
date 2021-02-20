<template>
  <div>
    <h1>Select user</h1>
    <input v-model="userId" type="text" @change="onLoadUser">
  </div>
</template>

<script>
export default {
  data () {
    return {
      userId: ''
    }
  },
  methods: {
    onLoadUser () {
      this.$router.push('/users/' + this.userId)
    }
  }
}
</script>

<style scoped></style>
