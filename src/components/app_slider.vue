<script>

import app_comics from '../app_comics.js';

  export default{
    name: 'app_slider',

    props: {
      img: String,
      name: String
    },

    data(){
      return{
        app_comics
      }
    }
  }
</script>

<template>
    <div class="current_series">
      <button><strong>CURRENT SERIES</strong></button>
    </div>

    <div class="films d-flex flex-wrap justify-content-around">
      <div>
        <comic v-for="comic in app_comics"
        :img="comic.thumb"
        :name="comic.series" />
      </div>

      <div>
        <img :src="thumb">
        <h1>{{name}}</h1>
      </div>
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
  height: 70vh;
  padding: 0 calc(35% / 2);
  background-color: $slider-bg-black;
}
</style>