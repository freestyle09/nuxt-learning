<template>
  <nuxt-link :to="'/posts/' + id">
    <article class="post-preview">
      <div class="post-thumbnail">
        <img :src="thumbnail" alt="">
      </div>
      <div class="post-content">
        <h1>{{ title }}</h1>
        <p>{{ previewText }}</p>
      </div>
    </article>
  </nuxt-link>
</template>

<script>
export default {
  props: {
    id: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    previewText: {
      type: String,
      required: true
    },
    thumbnail: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped lang="scss">
.post-thumbnail {
  box-shadow: 0 3px 6px rgba(0,0,0,.16);
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
</style>
