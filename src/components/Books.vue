<template class="yolo">
  <div class="books">
    <h2>Books</h2>
    <div class="list-books">
      <div v-bind:key="book.id" v-for="book in books">
        <BookItem v-bind:book="book"/>
      </div>
    </div>
  </div>
</template>

<script>
import BookItem from './BookItem.vue'

export default {
  name: "Books",
  components: {
    BookItem
  },
  props: ["books"]
}
</script>

<style scoped>

.books{
  margin-top: 50px;
}

.list-books{
  flex-wrap: wrap;
  display: flex;
}

h2{
  text-align: center;
}
</style>