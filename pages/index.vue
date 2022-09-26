<template>
    <div class="background" :style="{ backgroundImage: 'url(images/7.png)' }">
        <div class="card">algorithmic experiments</div>
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Finger+Paint&display=swap');
.background {
    display: grid;
    place-items: center;
    height: 100vh;
    width: 100%;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    
}

.card {
    position: absolute;
    top: 400px;
    color: white;
    font-size: 4rem;
    font-style: italic;
    font-family: 'Finger Paint', cursive;
    transition: font-size 1s;
}

@media (max-width: 550px) {
    .card {
        font-size: 2.8rem;
    }
}

</style>