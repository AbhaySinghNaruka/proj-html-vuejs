<template>
  <div class="logos">
    <div class="container">
      <img class="brackets" src="@/assets/img/logo-5.png" alt="">
      <img src="@/assets/img/logo-1.png" alt="">
      <img src="@/assets/img/logo-2.png" alt="">
      <img src="@/assets/img/logo-3.png" alt="">
      <img src="@/assets/img/logo-4.png" alt="">
      <img class="brackets" src="@/assets/img/logo-5.png" alt="">
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
  .logos {
    padding: 100px 0;
    background-color: #EEF4ED;
    .container {
      width: 1120px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      .brackets {
        transform: scale(0.5);
      }
      img {
        height: 100%;
        transform: scale(.7);
        filter: opacity(.5);
      }
    }
  }
</style>
