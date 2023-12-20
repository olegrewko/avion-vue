<template>
    <div>
        <layout-header />
        <hero />
        <aboutbrand />
        <product4  />
        <ideas  />
        

    </div>
</template>
<script setup>

import LayoutHeader from "@/components/layout/Header.vue";
import Hero from "@/components/layout/Hero.vue";
import Aboutbrand from "@/components/layout/Aboutbrand.vue";
import Product4 from "@/components/layout/Product4.vue";
import Ideas from "@/components/layout/Ideas.vue";

</script>



<style lang="scss">
@import "./assets/styles/global.scss";
@import url('https://fonts.cdnfonts.com/css/satoshi');
@import url('https://fonts.cdnfonts.com/css/clash-display');
 body {
    margin: 0;
    padding: 0;
 }
 img {
    display: block;
    max-width: 100%;
 }                                                                                                
                                                
</style>
