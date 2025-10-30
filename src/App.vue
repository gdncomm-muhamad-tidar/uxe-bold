<template>
  <div class="wrapper">
    <NavMenu />
    <section id="home" class="hero-section">
      <div class="hero-content">
        <h1>Welcome to Bold</h1>
        <p>Your Next Generation Vue.js Application</p>
      </div>
    </section>
    <section class="page">
      <h1>Section</h1>
    </section>
  </div>
</template>

<script setup>
import NavMenu from './components/NavMenu.vue'
</script>

<style lang="scss">
@import '@blibli/blue-font/dist/blue-font-blibli';
@import '@blibli/blue-design-tokens/dist/tokens-default';
@import '@blibli/blue-dls-utils/dist/scss/responsive-mixins-helper';

.hero {
  &-section {
    height: 80vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    background: linear-gradient(135deg, #42b883 0%, #347474 100%);
    color: white;
  }
}
.page {
  display: flex;
  align-items: center;
  justify-content: center;
}
.page {
  &:not(:last-child) {
    margin-bottom: 100px;
  }
  &:last-child {
    padding-bottom: 100px;
  }
  @include mobile {
    overflow: hidden;
  }
  &__container {
    max-width: 1200px;
    margin: auto;
    @include mobile {
      padding: 0 16px;
    }
  }
}
</style>
