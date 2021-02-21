<template>
  <div class="admin-page">
    <section class="new-post">
      <button @click="$router.push('/admin/new-post')">
        Create new post
      </button>
    </section>
    <section class="existing-posts">
      <h1>Existing posts</h1>
      <PostList />
    </section>
  </div>
</template>

<script>
import PostList from '~/components/Posts/PostList'

export default {
  components: {
    PostList
  }
}
</script>

<style scoped></style>
