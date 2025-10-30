<template>
  <div class="wrapper">
    <!-- <NavMenu /> -->
    <!-- <section id="home" class="hero-section">
      <div class="hero-content">
        <h1>Welcome to Bold</h1>
        <p>Your Next Generation Vue.js Application</p>
      </div>
    </section>
    <section class="page">
      <h1>Section</h1>
    </section> -->
    <div class="order">
      <div class="order-title">Detail pesanan</div>
      <div class="amount">
        <div class="amount__list">
          <div class="amount__item">Total belanja (7 produk)</div>
          <div class="amount__detail">Rp 150.000</div>
        </div>
        <div class="amount__list">
          <div class="amount__item">Ongkos kirim</div>
          <div class="amount__detail">Rp 150.000</div>
        </div>
        <div class="amount__list">
          <div class="amount__item">Biaya platform</div>
          <div class="amount__detail">Rp 150.000</div>
        </div>
        <div class="amount__list">
          <div class="amount__item">Potongan Voucher & Promo</div>
          <div class="amount__detail">Rp 150.000</div>
        </div>
        <div class="amount__list amount__total">
          <div class="amount__item">Total pembayaran</div>
          <div class="amount__detail">Rp5.000.000</div>
        </div>
        <div class="amount__list">
          <div class="amount__item">Cashback</div>
          <div class="amount__detail">Rp5.000.000</div>
        </div>
        <div class="amount__list">
          <div class="amount__item">Blibli Tiket Points</div>
          <div class="amount__detail">120 poin</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// import NavMenu from './components/NavMenu.vue'
</script>

<style lang="scss">
@import '@blibli/blue-font/dist/blue-font-blibli';
@import '@blibli/blue-design-tokens/dist/tokens-default';
// @import '@blibli/blue-dls-utils/dist/scss/responsive-mixins-helper';

.wrapper {
  background-color: $blu-color-info-background-med;
  padding: 40px;
}

.order {
  position: relative;
  margin: 16px;
  padding: 32px 16px 16px;
  border-radius: 0 0 12px 12px;
  background-color: $blu-color-neutral-background-default;
  border-right: 1px solid $blu-color-neutral-border-med;
  border-bottom: 1px solid $blu-color-neutral-border-med;
  border-left: 1px solid $blu-color-neutral-border-med;  
  border-top: 1px solid $blu-color-neutral-border-med;  
  max-width: 360px;
  -webkit-mask-image: radial-gradient(circle at 50% -2px, transparent 10px, red 10.5px);
  // -webkit-mask-position: 50% -10px;
  -webkit-mask-size: 30px 100%;
  &-title {
    color: $blu-color-neutral-text-high;
    font: $blu-text-title-2;
    margin-bottom: 16px;
  }
  &-top {
    position: absolute;
    top: -16px;
    left: -1px;
    width: 101%;
    img {
      width: 100%;
    }
  }
}

.amount {
  &__list {
    display: flex;
    justify-content: space-between;
    gap: 8px;
  }
  &__item {
    color: $blu-color-neutral-text-med;
    font: $blu-text-body-1;
    padding: 6px 0;
  }
  &__detail {
    color: $blu-color-neutral-text-med;
    font: $blu-text-body-1;
    padding: 6px 0;
  }
  &__total {
    border-top: 1px dashed $blu-color-neutral-border-med;
    border-bottom: 1px dashed $blu-color-neutral-border-med;
    padding: 12px 0;
    margin: 16px 0;
    & .amount__item,
    & .amount__detail {
      font: $blu-text-title-2;
      color: $blu-color-neutral-text-high;
    }
  }
}
// .hero {
//   &-section {
//     height: 80vh;
//     display: flex;
//     align-items: center;
//     justify-content: center;
//     text-align: center;
//     background: linear-gradient(135deg, #42b883 0%, #347474 100%);
//     color: white;
//   }
// }
// .page {
//   display: flex;
//   align-items: center;
//   justify-content: center;
// }
// .page {
//   &:not(:last-child) {
//     margin-bottom: 100px;
//   }
//   &:last-child {
//     padding-bottom: 100px;
//   }
//   @include mobile {
//     overflow: hidden;
//   }
//   &__container {
//     max-width: 1200px;
//     margin: auto;
//     @include mobile {
//       padding: 0 16px;
//     }
//   }
// }
</style>
