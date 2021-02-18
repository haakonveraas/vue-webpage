<template>
  <header class="header">
    <div>
      <router-link class="navitem" to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/contact">Contact</router-link> |
      <router-link to="/reading">Reading List</router-link>
    </div>
  </header>
</template>

<script>

</script>

<style>
  .header {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
  }

  .header a {
    color: #fff;
    padding-right: 5px;
    text-decoration: none;
  }
</style>