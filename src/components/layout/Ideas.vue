<template>
    <div class="ideas">
        <div class="ideas-left">
            <div class="ideas-left__info">
                <div class="ideas-left__info-text">
                    <h2 class="ideas-left__info-title">It started with a small idea</h2>
                    <span class="ideas-left__info-desc">A global brand with local beginnings, our story begain in a small studio in South London in early 2014</span>
                </div>
                <a class="ideas-left__info-link" href="">View collection</a>
            </div>

        </div>
        <div class="ideas-right">
            <img class="ideas-right-img" src="" alt="">
        </div>
    </div>
</template>
<style lang="scss" scoped>
.ideas {
    width: 1440px;
    height: 600px;
    background: #fff;

    display: flex;
    align-items: center;
    justify-content: center;
    padding: 60px 80px;

  
 &-left {
      background: #2A254B;  
      width: 634px;
      height: 478px;
      margin-right: 10px;

    &__info {
        background: #2A254B;
        margin-right: 16px;
        // display: flex;
        // flex-direction: column;
        // justify-content: space-between;
        display: flex;
        padding: 14px 35px 14px 35px;
        flex-direction: column;
        justify-content: flex-end;
        align-items: flex-start;
        gap: 205px;

        &-text {
            text-align: left;
        }

        &-title {
            text-align: left;
            color: #fff;

            /* Headings / H3 */
            font-family: Clash Display;
            font-size: 24px;
            font-style: normal;
            font-weight: 400;
            line-height: 140%;
            /* 33.6px */
        }

        &-desc {
            text-align: left;
            color: #fff;

            /* Body / Large */
            font-family: Satoshi;
            font-size: 18px;
            font-style: normal;
            font-weight: 400;
            line-height: 150%;
            /* 27px */
        }

        &-link {
            background: rgba(249, 249, 249, 0.15);
            text-align: left;
            display: flex;
            justify-content: center;
            padding: 16px 32px;
            align-items: center;
            gap: 10px;
            width: 170px;
            height: 56px;
            color: #fff;
            text-decoration: none;
            cursor: pointer;
            transition: all .3s;

            &:hover {
                background: rgba(249, 249, 249, 0.1);
                text-decoration: underline;
                cursor: pointer;
                transition: all .3s;
            }
        }
    }
}
&-right {
    width: 634px;
    height: 478px;
    background: url(/img/ImageBlock.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    &-img {
        min-width: 100%;
    }
}
}
</style>