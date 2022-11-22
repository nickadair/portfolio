<template>
    <div id="hex-container">
        <div id="hex">
            <slot name="image"></slot>
        </div> 
    </div>     
</template>

<style scoped>
    #hex-container::before,
    #hex-container::after {
        content: '';
        border-left: solid 2px gray;
        position: relative;
        left: 150px;
    }
    
    #hex {
        background-color: green;
        clip-path: polygon(25% 0%, 75% 0%, 100% 50%, 75% 100%, 25% 100%, 0% 50%);
        line-height: 0;
        margin: 0;
        padding: 0;
    }

    #hex img {
        margin: 0;
        padding: 0;
    }
</style>