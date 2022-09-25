<script setup>

</script>

<template>
    <div>
        <div class="profile">
            <img src="/images/profile.jpg">
        </div>
        
        <div class="about-div">
            <ContentDoc path="/about/"/>
        </div>  

    </div>
</template>

<style scoped>
.profile {
    display: grid;
    grid-auto-rows: 300px;
    place-items: center;
}

img {
    width: 200px;
    border-radius: 50%;
}

.about-div {
    line-height: 30px;
}

@media (min-width: 800px) {
  .about-div {
      margin-left: 25%;
      margin-right: 25%;
  }
}
</style>