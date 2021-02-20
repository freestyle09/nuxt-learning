<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest news!</h1>

      <section class="featured-posts">
        <PostPreview
          id="234"
          title="Barak Obama jaja obama"
          preview-text="lorem ipsum sit dolores"
          thumbnail="https://www.monsterenergy.com/media/uploads_image/2019/09/09/1600/800/6ea650cb9a77f4ac03b1c87fd8b21429.jpg?mod=v1_0485ae83b33a11d39f357c0a1ad1802f"
        />
        <PostPreview
          id="22"
          title="Lorem ipsum sit dolores"
          preview-text="lorem ipsum sit dolores"
          thumbnail="https://femefun.com/contents/videos_screenshots/46000/46172/preview.jpg"
        />
        <PostPreview
          id="209020094"
          title="Box sizing is very fun"
          preview-text="lorem ipsum sit dolores"
          thumbnail="https://www.nakedgirls.mobi/contents/videos_screenshots/4000/4191/preview.mp4.jpg"
        />
      </section>
    </section>
  </div>
</template>

<script>
import PostPreview from '~/components/Posts/PostPreview'

export default {
  components: {
    PostPreview
  }
}
</script>

<style lang="scss" scoped>
.featured-posts {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(0, 1fr));
  gap: 1rem
}
</style>
