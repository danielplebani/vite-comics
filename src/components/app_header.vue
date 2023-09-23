<script>
  export default{
    name: 'app_header'
  }
</script>

<template>
  <div class="d-flex justify-content-between align-items-center">
    <div class="col-2">
      <img src="../assets/img/dc-logo.png" alt="logo">
    </div>

    <div style="height: 100%;" class="col d-flex justify-content-end">
      <a href="#">CHARACTERS</a>
      <a href="#" class="active">COMICS</a>
      <a href="#">MOVIES</a>
      <a href="#">TV</a>
      <a href="#">GAMES</a>
      <a href="#">COLLECTIBLES</a>
      <a href="#">VIDEOS</a>
      <a href="#">FANS</a>
      <a href="#">NEWS</a>
      <a href="#">SHOP</a>
    </div>
  </div> 
</template>

<style lang="scss" scoped>
@use '../components/app_color.scss' as *;

img{
  width: 42%;
}

a{
  font-size: x-small;
  margin: 0 10px;
  height: 100%;
  display: flex;
  align-items: center;
  text-decoration: none;
  text-align: center;
  color: black;
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: bold;
}

.active{
  color: $main-card-bg-blue;
  border-bottom: 5px solid $main-card-bg-blue;
  padding-top: 5px;
}
</style>