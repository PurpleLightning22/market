<template >
  <div class="banner">
    <div class="banner-content">
      <h1>Stan Smith<span>, <br>Forever!</span></h1>
      <a href="#">Купить</a>
    </div>
  </div>
</template>
<script>
export default {

}
</script>
<style lang="scss">
.banner {
  background: #F4EFE9 url('@/assets/images/banner-bg.png') center center no-repeat;
  background-position: 100% 0;
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 45px 60px 0 60px;
  border-radius: 20px;
  padding-left: 60px;
  min-height: 300px;


  &::before {
    content: url('@/assets/images/corporations.png');
    position: absolute;
    top: 16px;
    left: 20px;
  }

  &-content {
    display: flex;
    flex-direction: column;
    gap: 11px;

    h1 {
      font-weight: 700;
      font-size: 38px;
      line-height: 46px;
      color: #8BB43C;

      span {
        color: #000;
        font-weight: 700;
      }
    }

    a {
      background: #A5D364;
      border-radius: 110px;
      padding: 14px 60px;
      width: max-content;
      font-weight: 700;
      font-size: 16px;
      line-height: 19px;
      text-align: center;
      text-transform: uppercase;
      color: #FFFFFF;
      text-decoration: none;
    }
  }
}
</style>