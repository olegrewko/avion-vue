<template>
    <div class="footer">
        <div class="footer-content">
            <div class="footer-content-top">
                <div class="footer-content-top-menu">
                    <div class="footer-content-top-menu__columns">
                        <div class="footer-content-top-menu__column">
                            <span class="footer-content-top-menu__column_title">Menu</span>
                            <span class="footer-content-top-menu__column_link">New arrivals</span>
                            <span class="footer-content-top-menu__column_link">Best sellers</span>
                            <span class="footer-content-top-menu__column_link">Recently viewed</span>
                            <span class="footer-content-top-menu__column_link">Popular this week</span>
                            <span class="footer-content-top-menu__column_link">All products</span>
                        </div>
                        <div class="footer-content-top-menu__column">
                            <span class="footer-content-top-menu__column_title">Categories</span>
                            <span class="footer-content-top-menu__column_link">Crockery</span>
                            <span class="footer-content-top-menu__column_link">Furniture</span>
                            <span class="footer-content-top-menu__column_link">Homeware</span>
                            <span class="footer-content-top-menu__column_link">Plant pots</span>
                            <span class="footer-content-top-menu__column_link">Chairs</span>
                            <span class="footer-content-top-menu__column_link">Chairs</span>
                        </div>
                        <div class="footer-content-top-menu__column">
                            <span class="footer-content-top-menu__column_title">Our company</span>
                            <span class="footer-content-top-menu__column_link">About us</span>
                            <span class="footer-content-top-menu__column_link">Vacancies</span>
                            <span class="footer-content-top-menu__column_link">Contact us</span>
                            
                        </div>
                    </div>

                    <div class="footer-content-top-menu__subscribe">
                        <span class="footer-content-top-menu__column_title">Join our mailing list</span>
                        <form class="footer-content-top-menu__form">
                                <input class="footer-content-top-menu__form_input" type="text" placeholder="youremail">
                                <button class="footer-content-top-menu__form_btn">Sign up</button>
                        </form>
                    </div>
                    
                </div>
                <!-- <div class="footer-content-top-menu__subscribe">
                <span class="footer-content-top-menu__column_title">Join our mailing list</span>
                <form class="footer-content-top-menu__form">
                        <input class="footer-content-top-menu__form_input" type="text" placeholder="youremail">
                        <button class="footer-content-top-menu__form_btn">Sign up</button>
                </form>
                </div> -->

            </div>
            
            <div class="footer-content-bottom">
                <div class="footer-content-bottom__copyright">
                    Copyright 2022 Avion LTD
                </div>

                <div class="footer-content-bottom__social">
                    <a class="footer-content-bottom__social_link" href="">
                        <img src="../../../public/svg/Logo--linkedin.png" alt="Logo--linkedin.svg">
                    </a> 
                    <a class="footer-content-bottom__social_link" href="">
                        <img src="../../../public/svg/facebook.svg" alt="Logo--linkedin.svg">
                    </a> 
                    <a class="footer-content-bottom__social_link" href="">
                        <img src="../../../public/svg/Logo--instagram.svg" alt="Logo--linkedin.svg">
                    </a> 
                    <a class="footer-content-bottom__social_link" href="">
                        <img src="../../../public/svg/Logo--skype.svg" alt="Logo--linkedin.svg">
                    </a> 
                    <a class="footer-content-bottom__social_link" href="">
                        <img src="../../../public/svg/Logo--twitter.svg" alt="Logo--linkedin.svg">
                    </a> 
                    <a class="footer-content-bottom__social_link" href="">
                        <img src="../../../public/svg/Logo--pinterest.svg" alt="Logo--linkedin.svg">
                    </a> 
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
 .footer {
    max-width: 1440px;
    height: 380px;
    background: #2A254B;
    color: #fff;

    &-content {
        padding: 50px 80px 20px 80px;
    &-top {
        
        border-bottom: 1px solid #4E4D93;
        &-menu {
            display: grid;
            grid-template-columns: 1fr 1fr;
            column-gap: 10px;
              @media screen and (max-width: 1024px){
       
                        grid-template-columns:  1fr ;
                        gap: 5px;
                    }

            &__columns {
                display: grid;
                grid-template-columns: repeat(3, 1fr);
                  @media screen and (max-width: 1024px){
       
                        grid-template-columns: repeat (2, 1fr );
                        gap: 5px;
                    }
               
            }
            &__column {
                display: block;
                    &_title {
                        display: block;
                        color:  #FFF;
                        
                        font-family: 'Clash Display', sans-serif;
                        font-size: 16px;
                        font-style: normal;
                        font-weight: 300;
                        line-height: normal;
                        margin-bottom: 10px;
                    }
                    &_link {
                        display: block;
                        color:  #FFF;
                        font-family: 'Satoshi', sans-serif;
                        font-size: 14px;
                        font-style: normal;
                        font-weight: 300;
                        line-height: normal;
                        margin-bottom: 10px;
                    }

                }
            &__subscribe {
                display: flex;
                flex-direction: column;
                justify-content: flex-start;
            }    
            &__form {
                 display: flex;
                justify-content: center;
                align-items: center;
            &_input {
                width: 509px;
                height: 56px;
                display: flex;
                padding: 17px 205px 17px 32px;
                align-items: center;
                flex: 1 0 0;
                align-self: stretch;
            }
            &_btn {
                width: 118px;
                height: 56px;
                display: flex;
                padding: 16px 32px;
                align-items: flex-start;
                gap: 10px;
                background: #fff;
                color: #2A254B;
            }
            }

        }
    }
   
    &-bottom {
        padding-top: 20px;
        display: flex;
        justify-content: space-between;

        &__copyright {
            color: var(--White, #FFF);
            font-family: 'Satoshi';
            font-size: 14px;
            font-style: normal;
            font-weight: 400;
            line-height: normal;
        }
        &__social {
            display: flex;
            justify-content: space-between;
            &_link {
              width: 24px;
              height: 24px;
              margin-right: 10px;  
            }
        }
    }
 }
 }
</style>