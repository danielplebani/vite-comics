<script>
export default{
  name: 'app_card_markup',

  data(){
        return{
            cards: [
                {
                    name: 'DIGITAL COMICS',
                    img: 'src/assets/img/buy-comics-digital-comics.png'
                },
                {
                    name: 'DC MERCHANDISE',
                    img: 'src/assets/img/buy-comics-merchandise.png'
                },
                {
                    name: 'SUBSCRIPTION',
                    img: 'src/assets/img/buy-comics-subscriptions.png'
                },
                {
                    name: 'COMIC SHOP LOCATOR',
                    img: 'src/assets/img/buy-comics-shop-locator.png'
                },
                {
                    name: 'DC POWER VISA',
                    img: 'src/assets/img/buy-dc-power-visa.svg'
                }
            ]
        }
    }
  
}
</script>

<template>
   <div class="d-flex align-items-center">
      <div class="col d-flex justify-content-center" v-for="card in cards">
        <img :src="card.img" class="me-2">
        <span>{{card.name}}</span>
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