<script setup>

</script>

<template>
    <div>
        <div class="profile">
            <img src="/images/profile.jpg">
        </div>
        
        <ContentDoc path="/about/"/>  

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

div {
    line-height: 30px;
}

@media (min-width: 800px) {
  div {
      margin-left: 25%;
      margin-right: 25%;
  }
}
</style>