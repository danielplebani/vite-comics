<script>
  export default{
    name: 'app_main_card',
  }
</script>

<template>
  <div class="d-flex">
   <div class="col d-flex">
     <img src="../assets/img/buy-comics-digital-comics.png">
     <span>DIGITAL COMICS</span>
   </div>

   <div class="col d-flex">
     <img src="../assets/img/buy-comics-merchandise.png">
     <span>DC MERCHANDISE</span>
   </div>

   <div class="col d-flex">
     <img src="../assets/img/buy-comics-subscriptions.png" >
     <span>SUBSCRIPTION</span>
   </div>

   <div class="col d-flex">
     <img src="../assets/img/buy-comics-shop-locator.png">
     <span>COMIC SHOP LOCATOR</span>
   </div>

   <div class="col d-flex">
     <img src="../assets/img/buy-dc-power-visa.svg">
     <span>DC POWER VISA</span>
   </div>
  </div>
</template>

<style scoped>
img{
  width: 40px;
}

span{
  font-family: 'Roboto Condensed', sans-serif;
  color: white;
}
</style>