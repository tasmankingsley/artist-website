<script setup>

let display_img = reactive({
    src: '',
    visible: false
})

function display(src) {
    display_img.src = src;
    display_img.visible = true;
}
    
</script>

<template>
    <div>
        <div class="grid">
            <img src="/images/1.png" @click="display('/images/1.png')">
            <img src="/images/2.png" @click="display('/images/2.png')">
            <img src="/images/3.png" @click="display('/images/3.png')">
            <img src="/images/4.png" @click="display('/images/4.png')">
            <img src="/images/5.png" @click="display('/images/5.png')">
            <img src="/images/6.png" @click="display('/images/6.png')">
            <img src="/images/7.png" @click="display('/images/7.png')">
            <img src="/images/8.png" @click="display('/images/8.png')">
            <img src="/images/9.png" @click="display('/images/9.png')">
            <img src="/images/10.png" @click="display('/images/10.png')">
            <img src="/images/11.png" @click="display('/images/11.png')">
            <img src="/images/12.png" @click="display('/images/12.png')">
        </div>
        <div class="display" v-if="display_img.visible" :style="{backgroundImage: `url(${display_img.src})`}" @click="display_img.visible = false"></div>
    </div>
</template>

<style scoped>
.grid {
    display: grid;
    grid-auto-flow: row;
    grid-template-columns: repeat(2, 1fr);
    gap: 10px;
}

img {
    width: 100%;
    height: auto;
    cursor: pointer;
}

.display {
    position: fixed;
    z-index: 10;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
    background-color: rgba(0, 0, 0, 0.95);
}

@media (min-width: 600px) {
    .grid {
        grid-template-columns: repeat(3, 1fr);
        gap: 10px;
    }
}

@media (min-width: 1000px) {
    .grid {
        grid-template-columns: repeat(4, 1fr);
    }
}
</style>