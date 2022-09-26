<script setup>

</script>

<template>
    <div>
        <div class="profile">
            <img class="profile-img" src="/images/profile.jpg">
        </div>
        
        <div class="about-div">
            <ContentDoc path="/about/"/>
        </div>  

    </div>
</template>

<style>
.profile {
    display: grid;
    grid-auto-rows: 300px;
    place-items: center;
}

ul {
  line-height: 50px;
}

a {
  /* text-decoration: none; */
  color: #191a21;
  /* text-decoration-color: #639ef3; */
}

h1 {
  color: coral;
  font-size: 40px;
  line-height: 40px;
}

.profile-img {
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