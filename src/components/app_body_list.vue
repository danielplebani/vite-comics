<script>
  export default{
    name: 'app_body_list',

    data(){
        return{
            DCcomics:['Characters','Comics','Movies','Tv','Games','Videos','News',],
            SHOP:['Shop DC','Shop DC collecctive'],
            DC:['Terms of use','Privacy police (news)','Movies','Tv','Games','Videos','News','News','News','News','News'],
            SITES:['DC','Mag magazine','DC Kids','DC university','DC power']
        }
    }
  }
</script>

<template>
    <div class="col-3 d-flex flex-column">
            <span class="my-2"><strong>DC COMICS</strong></span>
            <a href="#" v-for="element in DCcomics">{{element}}</a>

            <span class="my-2"><strong>SHOP</strong></span>
            <a href="#" v-for="element in SHOP">{{element}}</a>
    </div>

    <div class="col-3 d-flex flex-column">
                <span class="my-2"><strong>DC</strong></span>
            <a href="#" v-for="element in DC">{{element}}</a>
                
    </div>

    <div class="col-3 d-flex flex-column">
                <span class="my-2"><strong>SITES</strong></span>
                <a href="#" v-for="element in SITES">{{element}}</a>
    </div>
</template>

<style lang="scss" scoped>
a{
    color: gray;
    text-decoration: none;
    font-size: x-small;
    margin-bottom: 3px;
}
</style>