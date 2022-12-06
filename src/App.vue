<template>
  <div id="app">
    <HeaderPage />
  </div>
</template>

<script>
import HeaderPage from './components/HeaderPage.vue';

export default {
  name: 'App',
  components: {
    HeaderPage,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
  list-style: none;
  text-decoration: none;
}
</style>
