<template>
  <div >

              <ForumListItem v-for="(forum, index) in forums" :forum="forum" :key="index" />

          </div>
</template>

<script>
import ForumListItem from './ForumListItem'

export default {
  components: {
    ForumListItem
  },
  props: {
    forums: {
      required: true,
      type: Array
    }
  }
}
</script>