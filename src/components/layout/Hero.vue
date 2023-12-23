<template>
    <div class="hero">
          
                <div class="hero-info">
                    <div class="hero-info-text">
                    <h2 class="hero-info__title">Luxury homeware for people who love timeless design quality</h2>
                    <span class="hero-info__desc">Shop the new Spring 2022 collection today</span> 
                    </div>
                    <a class="hero-info-link" href="">View collection</a>
                </div>
                  
    </div>
</template>
<style lang="scss" scoped>
.hero {
    width: 1440px;
    height: 704px;
    background: url(/img/hero.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    padding-right: 50px;
    &-img {
        max-width: 100%;
    }
    &-info {
       background: #fff;
       max-width: 530px;
       padding: 50px 50px;
       height: 340px;
       display: flex;
       flex-direction: column;
       justify-content: space-between;
       
       &-text {
        text-align: left;
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