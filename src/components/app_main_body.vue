<script>

  import app_body_list from './app_body_list.vue';

  export default{
    name: 'app_main_body',

    components:{
        app_body_list
    }
  }
</script>

<template>
    <div class="d-flex text-white">
        <div class="col d-flex justify-content-start py-3">
            <app_body_list></app_body_list>
        </div>

        <div class="col logo">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.logo{
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: center;
    background-size: 450px;
}
</style>