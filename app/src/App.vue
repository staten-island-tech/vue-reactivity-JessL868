<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import ShopProduce from './components/ShopProduce.vue'
</script>

<template>
  <div class="shop">
    <h1>Nature's Basket</h1>
    <header>
      <ShopProduce/>
    </header>
  </div>

  <RouterView/>
</template>

<style scoped>
header {
  align-content:space-evenly;
}
h1{ 
  text-align: center;
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

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: 0rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  } 
}
</style>
