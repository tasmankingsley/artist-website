<script setup>

</script>

<template>
    <div>
        <img src="/images/1.png" >
        <img src="/images/2.png" >
        <img src="/images/3.png" >
        <img src="/images/4.png" >
        <img src="/images/5.png" >
        <img src="/images/6.png" >
        <img src="/images/7.png" >
        <img src="/images/8.png" >
    </div>
</template>

<style scoped>
div {
    display: grid;
    grid-auto-flow: row;
    grid-template-columns: repeat(4, 1fr);
    gap: 20px;
}

img {
    width: 100%;
    height: auto;
    cursor: pointer;
}
</style>