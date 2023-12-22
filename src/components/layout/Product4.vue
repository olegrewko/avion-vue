<template>
<div class="products-container">
    <div class="products">
        <Product
        v-for="product in products"
        :key="product.id"
        :img="product.img"
        :title="product.title"
        :price="product.price" />
     </div>
     <a class="products-link" href="">View more</a>
</div>
</template>
<script setup>
import {ref} from 'vue'
import Product from '@/components/layout/Product.vue'
const products = ref([
    {
        id: 0,
        img: '/img/p1.jpg',
        title: 'The Dandy chair',
        price: 250
    },
    {
        id: 1,
        img: '/img/p2.jpg',
        title: 'The Silky Vase',
        price: 125
    },
    {
        id: 2,
        img: '/img/p3.jpg',
        title: 'Rustic Vase Set',
        price: 150
    },
    {
        id: 3,
        img: '/img/p4.jpg',
        title: 'The Lucy Lamp',
        price: 155
    },
]);
</script>
<style lang="scss" scoped>
.products-container {
    margin: 0 auto;
    text-align: center;
    margin-bottom: 50px;
}
.products {
    display: flex;
    justify-content: space-between;
    // grid-template-columns: repeat (4, 1fr );
    gap: 20px;
    margin-bottom: 50px;
    @media screen and (max-width: 1024px){
        flex-wrap: wrap;
    grid-template-columns: repeat (2, 1fr );
    gap: 10px;
    }
    &-link {
        display: block;
        text-align: center;
        text-decoration: none;
        &:hover {
            text-decoration: underline;
        }
    }
}
</style>