<script setup lang="ts">
import { RouterLink, RouterView} from 'vue-router'
</script>


<template>

  <header>
     <div class="logo-container">
      <img alt= "logo" class="logo" src="./assets/icono.svg" width="350" height="350" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>
  <RouterView />
</template>

<style scoped>
 .logo-container {
  display: grid;
  place-content: center;
  text-align: center;
 }

 header {
  line-height: 1.5;
  max-height: 100vh;
}
</style>
