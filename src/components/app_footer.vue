<script>
  export default{
    name: 'app_footer'
  }
</script>

<template>
    <div class="d-flex justify-content-between align-items-center">
        <div class="col-2">
            <button><strong>SIGN-UP NOW!</strong></button>
        </div>

        <div class="col-4 d-flex justify-content-around">
            <span><strong>FOLLOW US</strong></span>
            <img src="../assets/img/footer-facebook.png" alt="facebook">
            <img src="../assets/img/footer-twitter.png" alt="facebook">
            <img src="../assets/img/footer-youtube.png" alt="facebook">
            <img src="../assets/img/footer-pinterest.png" alt="facebook">
            <img src="../assets/img/footer-periscope.png" alt="facebook">
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../components/app_color.scss' as *;

button{
    background-color: transparent;
    color: white;
    border-color: $main-card-bg-blue;
    padding: 10px;
    font-size: small;
}

span{
    color: $main-card-bg-blue;
    font-size: large;
    font-family: 'Roboto Condensed', sans-serif;
    align-self: flex-end;
}

img{
    width: 30px;
    aspect-ratio: 1 / 1;
}
</style>