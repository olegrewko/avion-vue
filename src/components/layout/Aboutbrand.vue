<template>
    <div class="about-brand">
        <h3 class="about-brand__title">What makes our brand different</h3>
        <div class="about-brand-elements">
            <div 
                class="about-brand-element"
                v-for="(e, i) in aboutbrands"
                :key="i">
                <img 
                class="about-brand-element__image" 
                :src="e.img" 
                :alt="e.title">
                <h4 class="about-brand-element__title">
                    {{ e.title }}
                </h4>
                <span class="about-brand-element__desc">
                    {{ e.desc }}
                </span>
            </div>
        </div>
    </div>
    
</template>
<script setup>
import {ref} from 'vue'
const aboutbrands = [
    {
        img: '/svg/delivery.svg',
        title: 'Next day as standard',
        desc: 'Order before 3pm and get your order the next day as standard'
    },
    {
        img: '/svg/Checkmark--outline.svg',
        title: 'Made by true artisans',
        desc: 'Handmade crafted goods made with real passion and craftmanship'
    },
    {
        img: '/svg/Purchase.svg',
        title: 'Unbeatable prices',
        desc: 'For our materials and quality you won’t find better prices anywhere'
    },
    {
        img: '/svg/Sprout.svg',
        title: 'Recycled packaging',
        desc: 'We use 100% recycled to ensure our footprint is more manageable'
    }
]
</script>
<style lang="scss">
.about-brand {
//    width: 1440px;
//    height: 476px; 
   padding: 80px 80px 130px 80px ;
   &__title {
    text-align: center;
    margin: 0 0 74px 0;
    color:  #2A254B;

    /* Headings / H3 */
    font-family: 'Clash Display';
    font-size: 24px;
    font-style: normal;
    font-weight: 400;
    line-height: 140%; /* 33.6px */
   }
   &-elements {
    
    display: grid;
    grid-template-columns: repeat(4, 320px);
    justify-content: space-between;
    gap: 10px;
    text-align: left;

  
    &__image {
        display: block;
        margin-bottom: 12px;
    }
    &__title {
        margin: 0 0 12px 0;
        color:  #2A254B;

        /* Headings / H4 */
        font-family: Clash Display;
        font-size: 20px;
        font-style: normal;
        font-weight: 400;
        line-height: 140%; /* 28px */
    }
    &__desc {
        margin: 0 0 12px 0;
        color:  #2A254B;
        text-align: left;
        /* Body/Medium */
        font-family: Satoshi;
        font-size: 16px;
        font-style: normal;
        font-weight: 400;
        line-height: 150%; /* 24px */
    }

   }
  
}
.about-brand-element {
    width: 280px;
    height: auto;
    padding: 30px;
    background-color: #F9F9F9;
}
</style>