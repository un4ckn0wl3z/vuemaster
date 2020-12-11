<template>
      <div class="post-list">
        <PostListItem v-for="(post,index) in posts" :key="index" :post="post"/>
      </div>
</template>

<script>
import PostListItem from './PostListItem'
export default {
  components: {
    PostListItem
  },
  props: {
    posts: {
      required: true,
      type: Array
    }
  }
}
</script>