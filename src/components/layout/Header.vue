<template>
  <header class="header">
    <div class="header-top">
        <div class="header-top-left">
            <div class="header-top-search">
             <img src="/svg/header-search.svg" alt="svg/header-search.svg">
            </div>
            <div class="header-top-mobile">
             <img src="/svg/menu-mobile.svg" alt="svg/menu-mobile.svg">
            </div>
        </div>
        <a class="header-logo" href="">Avion</a>
        <div class="header-top-right">
        <div class="header-top-right__cart" >
            <a href="">
            <img class="header-cart" src="/svg/header-cart.svg" alt="/svg/header-search.svg">
            </a>
        </div>
        <div class="header-top-right__user" >
            <a href="">
            <img class="header-user" src="/svg/header-user.svg" alt="/svg/header-user.svg">
            </a>
        </div>
        </div>
    </div>
    <div class="header-menu">
        <a class="header-menu__link" 
        :href="el.path"
        v-for="(el, i) of menu" :key="i">{{ el.name }}
        </a>
    </div>
    <router-link to="/"></router-link>
    <!-- <div class="header-menu-mobile">

    </div> -->
  </header>
</template>
<script setup>
import {ref} from 'vue'
const menu = [
    {
        name: 'Plant pots',
        path: '/plant'
    },
    {
        name: 'Ceramics',
        path: '/ceramics'
    },
    {
        name: 'Tables',
        path: '/tables'
    },
    {
        name: 'Chairs',
        path: '/chairs'
    },
    {
        name: 'Crockery',
        path: '/crockery'
    },
    {
        name: 'Tableware',
        path: '/tableware'
    },
    {
        name: 'Cutlery',
        path: '/cutlery'
    },
]
</script>
<style lang="scss" scoped>
.header {
  position: relative;
  background: #fff;
  font-weight: bold;
  padding: 0 10px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.07);
  max-width: 1440px;
  min-height: 132px;

//   display: flex;
//   align-items: center;
//   z-index: 1;
//   position: relative;
  &-top {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
    margin: 0 20px;
    min-height: 70px;
     @media screen and (max-width: 767px){
      height: auto;  
      margin: 0;
      display: flex;
      justify-content: space-between;  
    }
    &-left {
        display: flex;
        justify-content: space-between; 
    }
    &-mobile {
        display: none;
         @media screen and (max-width: 767px){
            display: block;
            height: auto;  
            margin: 0;
         
    }
    }
    &-search {
        display: flex;
        justify-content: start;
         @media screen and (max-width: 767px){
     order: 2;  
    }
    }
    &-right {
        display: flex;
        align-items: center;
        justify-content: flex-end;
           @media screen and (max-width: 767px){
            display: none;
            }
        &__user {
            margin-left: 10px;
        }
    }
  }
  &-logo {
    color: #22202E;
    font-family: 'Satoshi', sans-serif;
    font-size: 24px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    text-decoration: none;
    text-align: center;
     @media screen and (max-width: 767px){
            order: 1;
            }
    &:hover {
        text-decoration: underline;
    }
  }
  &-menu {
    background: #fff;
    font-weight: bold;
    // padding: 0 20px;
    color: #22202E;
    height: 62px;
    display: flex;
    justify-content: center;
    align-items: center;
     @media screen and (max-width: 767px){
      display: none;  
      border: none;  
    }
    &-mobile {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        padding: 40px 20px;
        &__link {
            display: block;
        }
    }
    &__link {

        margin: 0 20px;
        color: #22202E;
        text-decoration: none;
        cursor: pointer;
        transition: all .3s;
        &:hover {
            text-decoration: underline;
            cursor: pointer;
            transition: all .3s;
        }
    }
   
  }
}
</style>