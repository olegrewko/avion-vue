<template>
    <div class="subscribe">
    <div class="subscribe-content">
        <h3 class="subscribe-content-title">Join the club and get the benefits</h3>   
        <span class="subscribe-content-desc">Sign up for our newsletter and receive exclusive offers on new ranges, sales, pop up stores and more</span> 
         <div class="subscribe-content-checks">
         <div class="subscribe-content-check">
            <img class="subscribe-content-check__icon" src="../../../public/img/Checkmark--filled.svg" alt="Checkmark--filled.svg">
            <span class="subscribe-content-check__name">Exclusive offers</span>
         </div>
          <div class="subscribe-content-check">
            <img class="subscribe-content-check__icon" src="../../../public/img/Checkmark--filled.svg" alt="Checkmark--filled.svg">    
            <span class="subscribe-content-check__name">Free events</span>
          </div>
           <div class="subscribe-content-check">
            <img class="subscribe-content-check__icon" src="../../../public/img/Checkmark--filled.svg" alt="Checkmark--filled.svg">  
            <span class="subscribe-content-check__name">Large discounts</span>
         </div> 
         </div>
         <form class="subscribe-content-form">
            <input class="subscribe-content-form__input" type="text" placeholder="youremail">
            <button class="subscribe-content-form__btn">Sign up</button>
         </form> 
    </div>
    </div>
</template>
<style lang="scss" scoped>
.subscribe {
    max-width: 1440px;
    min-height: 440px;
    background: #474646;

    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0px 0px;
    margin: 0 100px 0 0;
    &-content {
        max-width: 600px;
        margin: auto;

    
     &-title {
        color:  #FFF;
        text-align: center;

        /* Headings / H2 */
        font-family: Clash Display;
        font-size: 32px;
        font-style: normal;
        font-weight: 400;
        line-height: 140%; /* 44.8px */

     }
     &-desc {
        color:  #FFF;
        text-align: center;
        /* Body / Large */
        font-family: Satoshi;
        font-size: 16px;
        font-style: normal;
        font-weight: 300;
        line-height: 150%; /* 27px */
        margin-bottom: 30px;
     }
     &-checks{
        display: flex;
        justify-content: center;
        margin-bottom: 20px;
     }
     &-check{
        display: flex;
        align-items: center;
        &:nth-child(2) {
            margin: 0 30px;
        }
        &__icon {
            margin-right: 10px;
        }
        &__name {
         color:  #FFF;
            text-align: center;
            font-family: Satoshi;
            font-size: 16px;
            font-style: normal;
            font-weight: 400;
            line-height: 150%; /* 24px */   
        }
        }
        &-form {
            display: flex;
            justify-content: center;
            align-items: center;
            &__input {
                display: flex;
                padding: 17px 205px 17px 32px;
                align-items: center;
                flex: 1 0 0;
                align-self: stretch;
            }
            &__btn {
                width: 118px;
                height: 56px;
                display: flex;
                padding: 16px 32px;
                align-items: center;
                gap: 10px;
                background: #2A254B;
                color: #FFF;
            }

        }
    }
}


</style>