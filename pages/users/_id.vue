<template>
  <h1>User ID is: {{ this.$route.params.id }}</h1>
</template>

<script>
export default {
  validate (data) {
    return /^\d+$/.test(data.params.id)
  }
}
</script>

<style scoped></style>
