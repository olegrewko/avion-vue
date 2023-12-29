<template>
    <div class="hero">
          
                <div class="hero-info">
                    <div class="hero-info-text">
                      <h2 class="hero-info__title">Luxury homeware for people who love timeless design quality</h2>
                      <span class="hero-info__desc">Shop the new Spring 2022 collection today</span> 
                    </div>
                    <button class="hero-info-btn">
                      <a class="hero-info-link" href="">View collection</a>
                    </button>
                                  
                </div>
                
                <img class="hero-min_img" src="/img/hb570.png" alt="/img/hb570.png">
               
    </div>
</template>
<style lang="scss" scoped>
.hero {
    max-width: 1440px;
    min-height: 704px;
    background: url(/img/hero.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    
    align-items: center;
    justify-content: flex-end;
    padding-right: 50px;
            @media screen and (max-width: 767px){
                height: auto;
                background: transparent;
                padding-right: 0;
                flex-direction: column;
                justify-content: flex-start;
            }
       
    &-min_img {
        display: none;
            @media screen and (max-width: 767px){
                display: block;
                order: 2;
            }
    }
    &-info {
       background: #fff;
       max-width: 630px;
       padding: 50px 50px;
       min-height: 340px;
       display: flex;
       flex-direction: column;
       justify-content: space-between;
       align-items: flex-start;
           @media screen and (max-width: 767px){
                padding: 40px 20px 20px 20px;
                min-height: 0;
                margin-top: 0;
                order: 1;
    }
       &-text {
                @media screen and (max-width: 767px){
                margin-bottom: 30px;
    }
}
       &-btn {
    background-color: lightgray;
    color: black;
    
    font-size: 12px;
    cursor: pointer;
    margin: 3px 0;
    border: none;
    display: flex;
    width: 337px;
    padding: 16px 32px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
        cursor: pointer;
     &:hover {
      background-color: white;
      transition: all 0.3s;
      border: none;
      transition: all 0.3s;
      cursor: pointer;  
    }
                @media screen and (max-width: 767px){
                width: 100%;
    }
       }
       &__title {
        text-align: left;
        color:  #2A254B;

        /* Headings / H3 */
        font-family: 'Clash Display';
        font-size: 24px;
        font-style: normal;
        font-weight: 400;
        line-height: 140%; /* 33.6px */
        }
        &__desc {
            text-align: left;
            color: #5B5676;

            /* Body / Large */
            // font-family: 'Satoshi';
            font-size: 18px;
            font-style: normal;
            font-weight: 400;
            line-height: 150%; /* 27px */
        }
        &-link {
            text-align: left;
            // display: flex;
            // justify-content: flex-start;
            // margin: 0 20px;
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