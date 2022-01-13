<template>
  <div class="main-content">
      <div class="jumbo">
          <img src="../assets/img/jumbotron.jpg" alt="">
      </div>
      <div class="container">
        <h1>--Content goes here--</h1>
      </div>
  </div>
</template>

<script>
export default {
    name: "Main",
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";

    .main-content {
        width: 100%;
        background-color: black;
    }

    .jumbo img{
        width: 100%;
        height: 400px;
        object-fit: cover;
        object-position: top;
    }
    
    h1 {
        color: white;
    }

    
</style>