<template>
  <div class="navbar">
    <nav>
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/products">Products</router-link></li>
        <li><router-link to="/about">About</router-link></li>
        <li><router-link to="/admin">Admin</router-link></li>
        <li><router-link to="/contact">Contact</router-link></li>
      </ul>
      <hr>
    </nav>
    <!-- <router-view/> -->
  </div>
</template>

<script>
  
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  nav {
    margin: auto;
  }
  h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
  hr {
    height: 30px;
    border-top: none;
    border-bottom: 2px solid black;
    width: 95vw;
    margin: auto;
  }
</style>