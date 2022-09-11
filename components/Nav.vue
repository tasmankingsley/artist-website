<script setup>

</script>

<template>
<div class="top-bar">
    <div class="title">tasman kingsley</div>
    <div class="nav">
        <div class="link">
            <NuxtLink to="/" active-class="active">Home</NuxtLink>
        </div>

        <div class="link">
            <NuxtLink to="/gallery" active-class="active">Gallery</NuxtLink>
        </div>

        <div class="link">
            <NuxtLink to="/blog" active-class="active">Blog</NuxtLink>
        </div>
        
        <div class="link">
            <NuxtLink to="/about" active-class="active">About</NuxtLink>
        </div>

    </div>
</div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Nothing+You+Could+Do&display=swap');
.top-bar {
    display: grid;
    grid-template-rows: repeat(2, 1fr);
    height: 100px;
    width: 100%;
    background-color: #fff;
    
}

.title {
    font-size: 1.8rem;
    text-align: center;
    place-self: center;
    font-weight: 300;
    font-family: 'Nothing You Could Do', cursive;
}

.nav {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    /* gap: 10px; */
    cursor: pointer;
}
.link {
    width: 100%;
    height: 100%;
    display: grid;
    place-items: center;


}

.link:hover, .link:active {
    
}

a, a:visited, a:hover, a:active {
    font-size: 1.5rem;
    font-weight: 300;
    height: 40px;
    line-height: 40px;
    width: 80%;
    border-radius: 5px;
    text-align: center;

    color: inherit;
    /* text-decoration: none; */
}

.active, a:hover {
    background-color: #dad9d4;
    border-radius: 5px;
    text-decoration: none;
}
</style>