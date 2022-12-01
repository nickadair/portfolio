<template>
    <div id="hex-container">
        <div id="hex">
            <slot name="image"></slot>
            <h2><slot name="text"></slot></h2>
        </div> 
    </div>     
</template>

<style scoped>
    #hex {
        background-color: green;
        clip-path: polygon(25% 0%, 75% 0%, 100% 50%, 75% 100%, 25% 100%, 0% 50%);
        line-height: 0;
        margin: 0;
        padding: 0;
        filter: grayscale(100%);
        transition: filter .75s ease;
    }

    #hex img {
        margin: 0;
        padding: 0;
    }

    #hex h2 {
        color: rgba(0, 0, 0, 0);
        text-shadow: 3px 3px 3px rgb(255, 255, 255);
        text-transform: uppercase;
        font-weight: bold;
        position: absolute;
        top: 50%;
        left:  50%;
        -webkit-transform: translate(-50%, -50%); /* iOS */
        transform: translate(-50%, -50%);
        transition-property: color;
        transition-duration: .75s;
        transition: color .75s ease, text-shadow .75s ease;
    }

    #hex:hover {
        filter: none;
    }

    #hex:hover h2 {
        color: rgb(255, 255, 255, 1.0);
        text-shadow: 0 0 1px black, 0 0 1px black, 0 0 1px black, 0 0 1px black; 
    }
</style>