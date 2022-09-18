<script setup>

onMounted(() => {
    const imgs = document.querySelectorAll('img');
    const fullPage = document.querySelector('.fullpage');

    imgs.forEach(img => {
    img.addEventListener('click', function() {
        fullPage.style.backgroundImage = 'url(' + img.src + ')';
        fullPage.style.display = 'block';
    });
    });
})

</script>

<template>
    <div>
        <div class="grid">
            <img src="/images/1.png" >
            <img src="/images/2.png" >
            <img src="/images/3.png" >
            <img src="/images/4.png" >
            <img src="/images/5.png" >
            <img src="/images/6.png" >
            <img src="/images/7.png" >
            <img src="/images/8.png" >
            <img src="/images/9.png" >
            <img src="/images/10.png" >
            <img src="/images/11.png" >
            <img src="/images/12.png" >
        </div>
        <div class="fullpage"></div>
    </div>
</template>

<style scoped>
.grid {
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

.fullpage {
  display: none;
  position: fixed;
  z-index: 99;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background-size: contain;
  background-repeat: no-repeat no-repeat;
  background-position: center center;
  background-color: black;
}
</style>