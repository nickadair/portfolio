<script setup>
import { RouterLink, RouterView } from 'vue-router';
import HexMenu from './components/HexMenu.vue';
</script>

<template>
  <header>
    <div class="title">
      <h2>Nikolas Adair</h2>
      <p class="vert">Web Developer</p>
    </div>  
    <div class="menu">
      <HexMenu v-if="$route.name!=='home'" />       
    </div>
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

  header {
    width: 90vw;
    display: flex;
    justify-content: space-between;
  }

  .menu {
    display: flex;
  }
}

@media (max-width: 767px) {
  main {
    display: block;
    position: absolute;
    top: 8rem;
    width: 100%;
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

  nav {
    margin: 0 auto;
  }
}
</style>
