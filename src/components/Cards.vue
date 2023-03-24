<template>
  <h2 class="title">Все кроссовки</h2>
  <div class="cards">
    <div class="cards-item">
      <img src="@/assets/images/kros-1.png" alt="">
      <p>Мужские Кроссовки Nike Blazer Mid Suede</p>
      <div>
        <h3><span>Цена:<br></span>12 999 руб.</h3>
        <div class="add">
          <input id="add" type="checkbox">
          <label for="add"></label>
        </div>

      </div>
    </div>
    <div class="cards-item">
      <img src="@/assets/images/kros-1.png" alt="">
    </div>
    <div class="cards-item">
      <img src="@/assets/images/kros-1.png" alt="">
    </div>
    <div class="cards-item">
      <img src="@/assets/images/kros-1.png" alt="">
    </div>
  </div>
</template>

<script>
export default {

}
</script>
<style lang="scss">
.cards {
  padding: 30px 60px;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 40px;

  &-item {
    background: #FFFFFF;
    border: 1px solid #F3F3F3;
    border-radius: 40px;
    padding: 20px 30px 34px 30px;
    display: flex;
    flex-direction: column;
    gap: 14px;

    img {
      width: 100%;
    }

    p {
      max-width: 150px;
      font-style: normal;
      font-weight: 400;
      font-size: 14px;
      line-height: 17px;
      color: #000000;
    }

    &>div {
      display: flex;
      align-items: center;
      justify-content: space-between;

      h3 {
        font-weight: 700;
        font-size: 14px;
        line-height: 17px;
        color: #000000;

        span {
          font-weight: 500;
          font-size: 11px;
          line-height: 13px;
          text-transform: uppercase;
          color: #BDBDBD;
        }
      }

      .add {
        position: relative;
        width: 32px;
        height: 32px;
        border: 1px solid #F2F2F2;
        border-radius: 8px;
        overflow: hidden;

        label {
          position: absolute;
          width: 100%;
          height: 100%;
          z-index: 1;


          &::before {
            content: url('@/assets/images/plus.svg');
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);

          }
        }

        input {
          opacity: 0;
          position: absolute;
          left: 0;
          top: 0;
          width: 100%;
          height: 100%;
          z-index: 2;
        }

        input:checked+label {
          background: linear-gradient(180deg, #89F09C 0%, #3CC755 100%);

          &::before {
            content: url('@/assets/images/true.svg');
          }


        }
      }

    }
  }
}
</style>