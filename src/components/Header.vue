<template>
  <header class="header">
    <a href="/" class="logo">
      <img src="@/assets/images/logo.png" alt="">
      <h3>REACT SNEAKERS<span>Магазин лучших кроссовок</span></h3>
    </a>
    <div class="header-content">
      <div class="header-content-basket">
        <img src="@/assets/images/basket.svg" alt="">
        <span>1205 руб.</span>
      </div>
      <div class="header-content-favourites">
        <img src="@/assets/images/fav.svg" alt="">
      </div>
      <div class="header-content-profile">
        <img src="@/assets/images/profile.svg" alt="">
      </div>
    </div>
  </header>
  <hr>
</template>
<script>
export default {

}
</script>
<style lang="scss">
.logo {
  display: flex;
  align-items: center;
  gap: 16px;
  text-decoration: none;
  color: #000;

  h3 {
    display: flex;
    flex-direction: column;
    font-weight: 700;
    font-size: 20px;
    line-height: 24px;
    color: #000000;

    span {
      font-weight: 400;
      font-size: 14px;
      line-height: 17px;

      color: #9D9D9D;

    }
  }
}

hr {
  background: #EAEAEA;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
  padding: 43px 60px;

  &-content {
    display: flex;
    align-items: center;
    gap: 30px;

    &-basket {
      display: flex;
      align-items: center;
      gap: 10px;

      span {
        font-weight: 600;
        font-size: 14px;
        line-height: 17px;
        color: #5C5C5C;

      }
    }
  }
}
</style>