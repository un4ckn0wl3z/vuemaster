<template>
  <div>
    <CategoryListItem v-for="(category, index) in categories" :key="index" :category="category" />
  </div>
</template>

<script>
import CategoryListItem from './CategoryListItem'

export default {
  props: {
    categories: {
      required: true,
      type: Array
    }
  },
  components: {
    CategoryListItem
  }
}
</script>