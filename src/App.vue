<template>
  <div id="app">
    <HeaderPage />
    <MainPage />
  </div>
</template>

<script>

import HeaderPage from './components/HeaderPage.vue';
import MainPage from './components/MainPage.vue';

export default {
  name: 'App',
  components: {
    HeaderPage,
    MainPage,
  },
};
</script>

<style lang="scss">

@import "~bootstrap/scss/bootstrap";

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Nunito Sans', sans-serif;
  list-style: none;
  text-decoration: none;

  .small-text {
    font-size: 15px;
    font-weight: 900;
    color: #00A6A6;
  }
  p {
    font-size: 18px;
    color: #6e6e6e;
}
}
</style>
