<script>
  export default{
    name: 'app_main_card',
  }
</script>

<template>
  <div class="d-flex align-items-center">
   <div class="col d-flex justify-content-center">
     <img src="../assets/img/buy-comics-digital-comics.png" class="me-2">
     <span>DIGITAL COMICS</span>
   </div>

   <div class="col d-flex justify-content-center">
     <img src="../assets/img/buy-comics-merchandise.png" class="me-2">
     <span>DC MERCHANDISE</span>
   </div>

   <div class="col d-flex justify-content-center">
     <img src="../assets/img/buy-comics-subscriptions.png"  class="me-2">
     <span>SUBSCRIPTION</span>
   </div>

   <div class="col d-flex justify-content-center">
     <img style="width: 30px;" src="../assets/img/buy-comics-shop-locator.png" class="me-2">
     <span>COMIC SHOP LOCATOR</span>
   </div>

   <div class="col d-flex justify-content-center">
     <img style="width: 45px;" src="../assets/img/buy-dc-power-visa.svg" class="me-2">
     <span>DC POWER VISA</span>
   </div>
  </div>
</template>

<style lang="scss" scoped>
img{
  width: 40px;
}

span{
  font-family: 'Roboto Condensed', sans-serif;
  color: white;
  align-self: center;
  font-size: small;
}
</style>