<script setup>
    
</script>

<template>
    <div class="blog-div">
        <ContentDoc path="/blog/"/>
    </div>
</template>

<style>
.blog-div {
  line-height: 30px;
}

ul {
  line-height: 50px;
}

a {
  color: coral;
  /* text-decoration: none; */
}

h1 {
  color: cadetblue;
}

@media (min-width: 800px) {
  .blog-div {
      margin-left: 25%;
      margin-right: 25%;
  }
}
</style>