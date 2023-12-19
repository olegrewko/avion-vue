<template>
    <div class="products">
    <Product
    v-for="product in products"
     :key="product.id"
     :img="product.img"
     :title="product.title"
     :price="product.price" />
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
        title: 'The Dandy chair',
        price: 125
    },
    {
        id: 2,
        img: '/img/p3.jpg',
        title: 'The Dandy chair',
        price: 150
    },
    {
        id: 3,
        img: '/img/p4.jpg',
        title: 'The Dandy chair',
        price: 155
    },
]);
</script>
<style lang="scss" scoped>
.products {
    display: grid;
    grid-template-columns: repeat (4, 1fr );
    gap: 20px;
}
</style>