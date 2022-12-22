<script setup>
import HexContainer from '../components/HexContainer.vue';
</script>

<template>
  <!-- <main> -->
    <div class="wrapper">
      <HexContainer class="left" url="about"> 
        <template #image>
          <img src="https://picsum.photos/300/280?random=1" alt="">
        </template>
        <template #text><RouterLink to="/">Home</RouterLink></template>
      </HexContainer>

      <HexContainer class="middle">
        <template #image>
          <img src="https://picsum.photos/300/280?random=2" alt="">
        </template>
        <template #text><RouterLink to="/work">Work</RouterLink></template>
      </HexContainer>

      <HexContainer class="right">
        <template #image>
          <img src="https://picsum.photos/300/280?random=3" alt="">
        </template>
        <template #text><RouterLink to="/contact">contact</RouterLink></template>
      </HexContainer>
      </div>
  <!-- </main> -->
</template>

<style scoped>
  .hex-container.left {
    top: -70px; 
    left: 70px;
  }

  .hex-container.middle {
    top: 70px;     
  }

  .hex-container.right {
    top: -70px; 
    left: -70px;
  }

  @media (max-width: 767px) {
    .hex-container.left {
    top: unset; 
    left: unset;
  }

  .hex-container.middle {
    top: unset;     
  }

  .hex-container.right {
    top: unset; 
    left: unset;
  }
}
</style>