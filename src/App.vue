<script setup>
import { RouterLink, RouterView } from 'vue-router'
import NavBar from './components/Navbar.vue'
</script>

<template>
  <header>
    <NavBar></NavBar>
  </header>
  <div class="wrapper">
    <RouterView />
  </div>
</template>

<style scoped>
  footer{
    margin-top: auto;
  }
  .wrapper {
    min-height:90vh;
  }
</style>
