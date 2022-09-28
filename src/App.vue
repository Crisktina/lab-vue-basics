<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="55" height="55" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/iteration2">iteration 2</RouterLink>
        <RouterLink to="/iteration3">iteration 3</RouterLink>
        <RouterLink to="/iteration4">iteration 4</RouterLink>
        <RouterLink to="/iteration5">iteration 5 Bonus</RouterLink>
      </nav>

  </header>

  <main>
    <RouterView />
  </main>
  
  <footer>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="50" height="25" />
    <p>Created by Cris ®</p>
  </footer>
</template>

<style scoped>


header {
  line-height: 1.5;
  max-height: 50vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
  margin-bottom: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
footer {
    margin-top: 3rem;
  }


  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
    margin-bottom: 2rem;
  }

  .logo {
    margin: 0 2rem 0 0;
  }


  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
  

</style>
