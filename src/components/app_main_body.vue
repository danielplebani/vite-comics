<script>
  export default{
    name: 'app_main_body'
  }
</script>

<template>
    <div class="d-flex text-white">
        <div class="col d-flex justify-content-start py-3">
            <div class="col-3 d-flex flex-column">
                <span class="my-2"><strong>DC COMICS</strong></span>
                <a href="#">Characters</a>
                <a href="#">Comics</a>
                <a href="#">Movies</a>
                <a href="#">Tv</a>
                <a href="#">Games</a>
                <a href="#">Videos</a>
                <a href="#">News</a>

                <span class="my-2"><strong>SHOP</strong></span>
                <a href="#">Shop DC</a>
                <a href="#">Shop DC collectibles</a>
            </div>
            <div class="col-3 d-flex flex-column">
                <span class="my-2"><strong>DC</strong></span>
                <a href="#">Terms of use</a>
                <a href="#">Privacy police (news)</a>
                <a href="#">Movies</a>
                <a href="#">Tv</a>
                <a href="#">Games</a>
                <a href="#">Videos</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
            </div>
            <div class="col-3 d-flex flex-column">
                <span class="my-2"><strong>SITES</strong></span>
                <a href="#">DC</a>
                <a href="#">Mag magazine</a>
                <a href="#">DC Kids</a>
                <a href="#">DC university</a>
                <a href="#">DC power</a>
            </div>
        </div>

        <div class="col logo">
        </div>
    </div>
</template>

<style lang="scss" scoped>
a{
    color: gray;
    text-decoration: none;
    font-size: x-small;
    margin-bottom: 3px;
}

.logo{
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: center;
    background-size: 450px;
}
</style>