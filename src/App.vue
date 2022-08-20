<script setup>
import { RouterLink, RouterView } from "vue-router";
import Header from "./components/Header.vue";
</script>

<template>
    <header>
    <RouterLink to="/"><h1>Cozinheiros</h1></RouterLink>
    <div class="wrapper">
      <nav>
        <RouterLink to="/about"> <a>sobre</a></RouterLink>
      </nav>
    </div>
  </header>
  <body>
  <RouterView />
  </body>
</template>

<style scoped>

header {
  background-color: #5F6873;
  line-height: 1.5; 
  max-height: 100vh
} 
nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color:#5F6873;
  background-color: #F28705;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(#F28705);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    display: flex;
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
    padding: 1rem 0;
    margin-top: 1rem;
  } 
}

</style>
