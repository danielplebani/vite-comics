<script>
  export default{
    name: 'app_header',

    data(){
      return{
        choices: [
          {
            name:'CHARACTERS',
            click:false
          },
          {
            name:'COMICS',
            click:true
          },
          {
            name:'MOVIES',
            click:false
          },
          {
            name:'TV',
            click:false
          },
          {
            name:'GAMES',
            click:false
          },
          {
            name:'COLLECTIBLES',
            click:false
          },
          {
            name:'VIDEOS',
            click:false
          },
          {
            name:'FANS',
            click:false
          },
          {
            name:'NEWS',
            click:false
          },
          {
            name:'SHOP',
            click:false
          }
        ],
      }
    },

    methods:{
      choiceClicked(index){
        for (let i = 0; i < this.choices.length; i++) {
          this.choices[i].click = false;
        }
        this.choices[index].click = true;
      }
    }
  }
</script>

<template>
  <div class="d-flex justify-content-between align-items-center">
    <div class="col-2">
      <img src="../assets/img/dc-logo.png" alt="logo">
    </div>

    <div style="height: 100%;" class="col d-flex justify-content-end">

      <div v-for="(choice, index) in choices">
        <a @click="choiceClicked(index)" :class="choice.click == true ? 'active' : '' " href="#">{{choice.name}}</a>
      </div>

    </div>
  </div> 
</template>

<style lang="scss" scoped>
@use '../components/app_color.scss' as *;

img{
  width: 42%;
}

a{
  font-size: x-small;
  margin: 0 10px;
  height: 100%;
  display: flex;
  align-items: center;
  text-decoration: none;
  text-align: center;
  color: black;
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: bold;
}

.active{
  color: $main-card-bg-blue;
  border-bottom: 5px solid $main-card-bg-blue;
  padding-top: 5px;
}
</style>