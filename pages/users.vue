<template>
  <div>
    <h1>Users page</h1>
    <p>This page is rendered everywhere in users path</p>
    <nuxt-child />
  </div>
</template>

<script>
export default {
  layout: 'users'
}
</script>

<style scoped></style>
