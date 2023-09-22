<script>
  import app_header from './components/app_header.vue'

  import app_slider from './components/app_slider.vue'

  import app_main_card from './components/app_main_card.vue'



  export default {
    components:{
      app_header,
      app_slider,
      app_main_card,
    },
    data(){
      return{
      }
    }
  }
</script>


<template>
  <app_header id="header"></app_header>
  <app_slider id="slider"></app_slider>
  <app_main_card id="main_card"></app_main_card>
</template>


<style lang="scss" scoped>
</style>
