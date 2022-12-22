<script setup>
import { RouterLink, RouterView } from 'vue-router';
</script>

<template>
  <header>
    <h2>Nikolas Adair</h2>
    <p class="vert">Web Developer</p>
  </header>

  <main>
    <nav><RouterView /></nav>
  </main>
</template>

<style scoped>
main {
  line-height: 1.5;
  max-height: 100vh;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
}

header {
  position: absolute;
  top: 5px;
}

header h2 {
  font-size: 3rem; 
  font-weight: 800;
}

header p.vert {
    writing-mode: vertical-rl;
  }

@media (min-width: 768px) {
  main {
    display: flex;
    place-items: center;
    margin: 0 auto;
  }

  main .wrapper {
    display: flex;
    place-items: flex-start;
    margin: 0 auto;
  }    
}

@media (max-width: 767px) {
  main {
    display: block;
  }

  main .wrapper {
    display: flex;
    place-items: center;
    flex-direction: column;
    gap: .5rem;
  }  

  header {
    position: unset;
    top: unset;
  }
}
</style>
