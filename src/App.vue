<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="app-container">
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/contact">Contact</RouterLink>
    </nav>
  

    <main>
      <RouterView />
    </main>
  </div>
</template>

<style scoped>
.app-container {
  max-width: 900px;
  margin: 0 auto;
  padding: 40px 20px;
}

nav {
  display: flex;
  gap: 20px;
  margin-bottom: 40px;
}

nav a {
  text-decoration: none;
  color: #8b5cf6;
  font-weight: bold;
}

nav a:hover {
  color: #c4b5fd;
}
</style>
