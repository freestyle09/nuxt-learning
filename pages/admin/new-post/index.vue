<template>
  <div class="admin-new-post">
    <section class="new-post">
      <form @submit.prevent="onSave">
        <AppControlInput v-model="editedPost.author">
          Author Name
        </AppControlInput>
        <AppControlInput v-model="editedPost.title">
          Title
        </AppControlInput>
        <AppControlInput v-model="editedPost.thumbnailLink">
          Thumbnail Link
        </AppControlInput>
        <AppControlInput v-model="editedPost.content" control-type="textarea">
          Content
        </AppControlInput>
        <Button type="submit">
          Save
        </Button>
        <Button
          type="button"
          style="margin-left: 10px"
          btn-style="cancel"
          @click="onCancel"
        >
          Cancel
        </Button>
      </form>
    </section>
  </div>
</template>

<script>
import Button from '@/components/Button'
import AppControlInput from '~/components/UI/AppControlInput'

export default {
  components: {
    Button,
    AppControlInput
  },
  data () {
    return {
      editedPost: {
        author: '',
        title: '',
        thumbnailLink: '',
        content: ''
      }
    }
  },
  methods: {
    onSave () {
      //  Save the post
    },
    onCancel () {
      //  Cancel the post
      this.$router.push('/admin')
    }
  }
}
</script>

<style scoped></style>
