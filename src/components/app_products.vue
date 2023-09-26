<script>
export default {
    name: 'app_products',

    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
    }

}
</script>



<template>
    <div class="product">
        <img :src="thumb">
        <p>{{ series }}</p>
    </div>
</template>



<style lang="scss" scoped>
@use '../app_color.scss' as *;
.product {
    display: flex;
    flex-direction: column;
    margin: 1rem 0;

    p {
        color: white;
        font-size: x-small;
        text-transform: uppercase;
    }

    img {
        width: 100%;
        aspect-ratio: 1;
        object-fit: cover;
        margin-bottom: 10px;
    }
}
</style>