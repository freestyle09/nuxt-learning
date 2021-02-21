<template>
  <section class="featured-posts">
    <PostPreview
      id="234"
      title="Barak Obama jaja obama"
      preview-text="lorem ipsum sit dolores"
      thumbnail="https://www.satellitetoday.com/wp-content/uploads/2019/06/Screen-Shot-2019-06-13-at-5.50.12-PM-800x490.png"
    />
    <PostPreview
      id="22"
      title="Lorem ipsum sit dolores"
      preview-text="lorem ipsum sit dolores"
      thumbnail="https://spacenews.com/wp-content/uploads/2018/05/24359364107_152b0152ff_k.jpg"
    />
    <PostPreview
      id="209020094"
      title="Box sizing is very fun"
      preview-text="lorem ipsum sit dolores"
      thumbnail="https://addons-media.operacdn.com/media/CACHE/images/themes/15/26915/12.0-rev1/images/9837a381-e1b3-49ff-a3b7-575cad21aaed/26d6fa48303cf571dec2d7be892b8899.jpg"
    />
  </section>
</template>

<script>
import PostPreview from '~/components/Posts/PostPreview'

export default {
  name: 'PostList',
  components: {
    PostPreview
  }
}
</script>

<style scoped></style>
