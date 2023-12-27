<template>
    <div class="product">
        <div class="product-center">
        <a href="">
            <img 
            class="product-image" 
            :src="img" 
            :alt="title">
        </a>
        <h4 class="product-name" href="">{{ title }}</h4>
        <span class="product-price">{{ price }}</span>
        </div>
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
        type: Number,
        required: true
    },
}) 

</script>
<style lang="scss" scoped>
.product {
    display: flex;
    justify-content: center;
    &-center {
        
        

    }
    &-image {
        display: block;
        text-align: center;
        margin: 5px;
        margin-bottom: 24px;
    }
    &-name {
        display: block;
        text-align: left;
        // padding: 0 80px;
        margin-bottom: 8px;
        color:  #2A254B;

        /* Headings / H4 */
        font-family: Clash Display;
        font-size: 20px;
        font-style: normal;
        font-weight: 400;
        line-height: 140%; /* 28px */
    }
    &-price {
        display: block;
        text-align: left;
        margin-bottom: 0px;
        color:  #2A254B;

        /* Headings / H4 */
        font-family: Clash Display;
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        line-height: 140%; /* 28px */
    }
}
</style>