<template>
    <div class="hero">
      <img src="/img/hero.jpg" alt="/img/hero.jpg">  
    </div>
    <div class="hero-info">
      <h2 class="hero-info__title">What makes our brand different</h2> 
    </div>
</template>
<style lang="scss" scoped>
.hero {
    // width: 1440px;
    height: 704px;
    // background: url(<path-to-image>), lightgray 50% / cover no-repeat;
    &__title {
        color: var(--Dark-Primary, #2A254B);

    /* Headings / H3 */
    font-family: Clash Display;
    font-size: 24px;
    font-style: normal;
    font-weight: 400;
    line-height: 140%; /* 33.6px */
    }
}
</style>