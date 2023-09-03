<script setup lang="ts">
import Footer from './components/FooterItem.vue'
</script>

<template>
  <div class="app">
    <header>
      <nav>
        <div class="block"><router-link to="/">Home</router-link></div>
        <div class="block"><router-link to="/about">About</router-link></div>
      </nav>
    </header>
    <router-view />
    <Footer />
  </div>
</template>

<style scoped>
nav {
  background-color: #ffffe2;
  color: rgb(255, 255, 255);
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 2rem;
  padding: 0 1rem;
}
.router-link-active{
  color: #000000;
  text-decoration: none;
}
a {
  color: #000000;
  text-decoration: none;
}
.block {
  padding: 1rem;
  border-radius: 0.5rem;
  background-color: #ffffd9;
  color: #000000;
}
.block:hover {
  background-color: #ffedbb;
  color: #ffffe2;
}
</style>
