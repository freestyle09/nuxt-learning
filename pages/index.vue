<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest news!</h1>
      <TheHeader />
    </section>
    <PostList />
  </div>
</template>

<script>
import TheHeader from '~/components/Navigation/TheHeader'
import PostList from '~/components/Posts/PostList'

export default {
  components: {
    TheHeader,
    PostList
  }
}
</script>

<style lang="scss" scoped>
.home-page {
  background-image: url("~/assets/images/sun.webp");
  background-size: cover;
  min-height: 100vh;
}
.featured-posts {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(0, 1fr));
  gap: 1rem;
}
</style>
