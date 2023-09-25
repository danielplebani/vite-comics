<script>

import app_comics from '../app_comics';

export default {
  name: 'app_slider',

  data() {
    return {
      app_comics
    }
  }
}
</script>

<template>
    <div class="current_series">
      <button><strong>CURRENT SERIES</strong></button>
    </div>

    <div class="films pt-5 pb-3 d-flex flex-column">
      <div class="container d-flex flex-wrap justify-content-around">
        <div v-for="comic in app_comics" :key="comic.series" class="mb-3">
          <img :src="comic.thumb" class="mb-3">
          <p>{{comic.series}}</p>
        </div>
      </div>

      <button><strong>LOAD MORE</strong></button>
    </div>

</template>

<style lang="scss" scoped>

@use '../app_color.scss' as *;

.current_series{
  height: 50vh;
  padding: 0 calc(35% / 2);
  background-image: url(../assets/img/jumbotron.jpg);
  background-size: cover;
  position: relative;

    button{
      border: none;
      color: white;
      background-color: $main-card-bg-blue;
      font-family: 'Roboto Condensed', sans-serif;
      padding: 5px 15px;
      position: absolute;
      bottom: -17px;
    }
}

.films{
  padding: 0 calc(35% / 2);
  background-color: $slider-bg-black;

  .container{
    div{
    width: calc(90% / 6);
      img{
        width: 100%;
        aspect-ratio: 1;
        object-fit: cover;
      }
      p{
        color: white;
        font-size: x-small;
        text-transform: uppercase;
      }
    }
  }

  button{
    border: none;
    color: white;
    background-color: $main-card-bg-blue;
    font-family: 'Roboto Condensed', sans-serif;
    font-size: x-small;
    padding: 5px 40px;
    text-align: center;
    margin: auto;
  }
}
</style>