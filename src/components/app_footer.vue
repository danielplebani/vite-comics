<script>
  export default{
    name: 'app_footer',

    data(){
        return{
            clickedButton: false,

            socials: [
                {
                    name: 'facebook',
                    img: 'src/assets/img/footer-facebook.png'
                },
                {
                    name: 'twitter',
                    img: 'src/assets/img/footer-twitter.png'
                },
                {
                    name: 'youtube',
                    img: 'src/assets/img/footer-youtube.png'
                },
                {
                    name: 'pinterest',
                    img: 'src/assets/img/footer-pinterest.png'
                },
                {
                    name: 'periscope',
                    img: 'src/assets/img/footer-periscope.png'
                }
            ]
        }
    },

    methods:{
        clickButton(){
            this.clickedButton = !this.clickedButton
        }
    }
  }
</script>

<template>
    <div class="d-flex justify-content-between align-items-center">
        <div class="col-2">
            <button @click="clickButton()" :class="clickedButton == true ? 'clickButton' : '' "><strong>SIGN-UP NOW!</strong></button>
        </div>

        <div class="col-4 d-flex justify-content-around">
            <span><strong>FOLLOW US</strong></span>
            <div v-for="social in socials">
                <img :src="social.img" :alt='social.name'>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../app_color.scss' as *;

button{
    background-color: transparent;
    color: white;
    border-color: $main-card-bg-blue;
    padding: 10px;
    font-size: small;
}

.clickButton{
    background-color: rgba(255, 255, 255, 0.044);
    color: $main-card-bg-blue;
    border: 2px solid $main-card-bg-blue;
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