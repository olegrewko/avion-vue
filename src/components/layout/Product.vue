<template>
    <div class="product">
        <a href="">
            <img 
            class="product-image" 
            :src="img" 
            :alt="title">
        </a>
        <a class="product-name" href="">{{ title }}</a>
        <span class="product-price">{{ price }}</span>
    </div>
</template>
<script setup>
const props = defineProps({
    img: {
        type: String,
        required: true
    },
    title: {
        type: String,
        required: true
    },
    price: {
        type: String,
        required: true
    },
}) 

</script>
<style lang="scss" scoped>
.product {
    &-img {
        display: block;
        margin-bottom: 24px;
    }
    &-name {
        display: block;
        padding: 0 80px;
        margin-bottom: 8px;
        color:  #2A254B;

        /* Headings / H4 */
        // font-family: Clash Display;
        font-size: 20px;
        font-style: normal;
        font-weight: 400;
        line-height: 140%; /* 28px */
    }
    &-price {
        display: block;
        margin-bottom: 0px;
        color:  #2A254B;

        /* Headings / H4 */
        // font-family: Clash Display;
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        line-height: 140%; /* 28px */
    }
}
</style>