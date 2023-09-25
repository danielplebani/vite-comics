<script>
  import app_header from './components/app_header.vue';
  import app_slider from './components/app_slider.vue';
  import app_main_card from './components/app_main_card.vue';
  import app_main_body from './components/app_main_body.vue';
  import app_footer from './components/app_footer.vue';

  export default {
    components:{
      app_header,
      app_slider,
      app_main_card,
      app_main_body,
      app_footer,
    }
  }
</script>


<template>
  <app_header id="header"></app_header>
  <app_slider id="slider"></app_slider>
  <app_main_card id="main_card"></app_main_card>
  <app_main_body id="main_body"></app_main_body>
  <app_footer id="footer"></app_footer>
</template>