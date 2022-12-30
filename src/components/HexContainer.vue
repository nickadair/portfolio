<template>
    <div class="hex-container">
        <div class="hex">
            <slot name="image"></slot>
            <div class="hex-inner">
                <slot name="text"></slot>
            </div>
        </div>
    </div>
</template>

<style scoped>
@media (max-width: 767px) {
    .hex {
        margin: 0 auto;
    }
}

.hex {
    background-color: white;
    clip-path: polygon(25% 0%, 75% 0%, 100% 50%, 75% 100%, 25% 100%, 0% 50%);
    line-height: 0;
    margin: 0;
    padding: 0;
    filter: grayscale(100%);
    transition: filter .75s ease;
}

.hex img {
    margin: 0;
    padding: 0;
}

.hex .hex-inner {
    position: absolute;
    top: 50%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    font-size: 1.5rem;
    text-decoration: none;
    text-transform: uppercase;
    color: white;    
}

.hex:hover {
    filter: none;
}
</style>