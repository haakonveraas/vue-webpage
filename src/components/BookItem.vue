<template>
  <div class="book-item">
    <h3>{{book.title}}</h3>
    <p class="author">{{book.author}}</p>
    <p>
      {{book.description}}
    </p>
    <div class="redirect" ><a href="">Read more</a></div>
  </div>
</template>

<script>
export default {
  name: "Book",
  props: ["book"]
}
</script>

<style scoped>
  .book-item .author{
    text-decoration: underline;
  }

  .book-item{
    background: #f4f4f4;
    padding: 10px;
    margin: 10px;
    width: 20rem;
    height: 20rem;
  }

  .redirect{
    top: 100px;
  }
</style>