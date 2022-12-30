<script setup>
    import HexContainer from '../components/HexContainer.vue';
</script>

<template>
    <HexContainer url="about">
        <template #image>
            <img src="https://picsum.photos/100/80?random=1" alt="">
        </template>
        <template #text>
            <RouterLink class="menu-link" to="/">Home</RouterLink>
        </template>
    </HexContainer>

    <HexContainer>
        <template #image>
            <img src="https://picsum.photos/100/80?random=2" alt="">
        </template>
        <template #text>
            <RouterLink class="menu-link" to="/work">Work</RouterLink>
        </template>
    </HexContainer>

    <HexContainer>
        <template #image>
            <img src="https://picsum.photos/100/80?random=3" alt="">
        </template>
        <template #text>
            <RouterLink class="menu-link" to="/contact">contact</RouterLink>
        </template>
    </HexContainer>
</template>
  