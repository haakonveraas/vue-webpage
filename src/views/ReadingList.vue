<template>
  <div class="reading">
    <h1>Reading List</h1>
    <div class="introduction">
      Here is a set of books and blogs that I like. I prefer books that give significant value to the reader. Books I don't recommend are those that
      spend too much time on building up the credibility of the author and his viewpoint. I'm also not a big fan of self-development books as I believe the authors exploit the insecurity of
      peoples strive for growth and that they almost everytime does not present enough value to live up to the expectations.
    </div>
    <Books v-bind:books="books"/>
  </div>
</template>

<script>
import Books from '../components/Books';

export default {
  name: "ReadingList",
  components: {
    Books
  },
  data(){
    return{
      books: [
        {
          id: 1,
          title: "Art and Craft of Problem Solving",
          author: "Paul Zeits",
          description: "Gives a brief introduction into the realms of Problem Solving.",
          form: "Book",
          type: "Mathematics"
        },
        {
          id: 2,
          title: "Valuation",
          author: "McKinsey",
          description: "Primer on valuation of companies",
          form: "Book",
          type: "Finance"
        },
        {
          id: 3,
          title: "Clean Code",
          author: "Robert Martin",
          description: "A great book on how to write well-structured, easy-to-read code. Examples in Java",
          form: "Book",
          type: "Programming"
        },
        {
          id: 4,
          title: "Clean Code",
          author: "Robert Martin",
          description: "A great book on how to write well-structured, easy-to-read code. Examples in Java",
          form: "Book",
          type: "Programming"
        }
      ]
    }
  }
}
</script>

<style scoped>
.reading{
  padding: 20px;
}
</style>