<script setup>
  import HexMenu from '../components/HexMenu.vue';
</script>

<template>
  <div class="worklist">
      <div class="light wide-tall">
        <img src="../assets/images/eekwi.org-old.jpeg" alt="" class="left">
        <img src="../assets/images/www.eekwi.org.jpeg" alt="" class="right">
      </div>
      <div class="dark wide-tall">
        <img src="../assets/images/www.tomahhealth.org-old.jpeg" alt="" class="left">
        <img src="../assets/images/www.tomahhealth.org.jpeg" alt="" class="right">
      </div>
      <div class="light wide-tall">
        <img src="../assets/images/neurology.wisc.edu-old.jpeg" alt="" class="left">
        <img src="../assets/images/neurology.wisc.edu.jpeg" alt="" class="right">
      </div>
  </div> 
</template>

<style>
@media (min-width: 768px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }

  .light {
    background-color: darkgray;
    color: black;
  }

  .dark {
    background-color: black;
    color: white;
  }

  .wide-tall {
    min-width: 100vw;
    width: 100vw;
  }

  .wide-tall img {
    width: 20%;
    height: 20%;
  }

  .worklist {
    margin-top: 10rem;
  }

  .right {
    margin-left: auto;
  }

  .left {
    margin-right: auto;
  }
}
</style>
