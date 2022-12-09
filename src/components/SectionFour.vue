<template>
  <div>
    <div class="container">
      <div class="top">
        <div class="small-text">OUR EDITORIAL CONTENT</div>
        <div class="news">
          <h1>Latest <span>News</span></h1>
        </div>
        <div class="top-btn">
          <div class="text">
            Every week we publish content about what is best in the business world.
          </div>
            <div class="button">SEE ALL</div>
        </div>
      </div>
      <div class="cards">
        <div class="card-container card-one">
          <div class="card-text">
            Increasing creativity is possible for everyone
          </div>
        </div>
        <div class="card-container card-two">
          <div class="card-text">
           Because market research is part of the business plan
          </div>
        </div>
        <div class="card-container card-three">
          <div class="card-text">
           Working from home is now a trend
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
.container {
  width: 1150px;
  height: 850px;
  padding: 130px 0;
  .news {
    margin: 25px 0;
    h1 {
      font-weight: 900;
      font-size: 55px;
      span {
        color: #058283;
        background-color: #DAECED;
        padding: 5px 10px;
        border-radius: 10px;
      }
    }
  }
  .top-btn{
    display: flex;
    justify-content: space-between;
    .text {
      font-size: 18px;
      color: #4f5050;
    }
    .button {
      color: white;
      background-color: #058283;
      padding: 8px 25px;
      border-radius: 5px;
      margin-bottom:50px
    }
    .button:hover{
      background-color:#CCE3DE;
      color: #058283;
      transition: .3s;
      cursor:pointer;
    }
  }
  .cards {
    display: flex;
    justify-content: space-between;
    gap: 30px;
    text-align: center;
    .card-container {
      width: calc(100%/3);
      border-radius: 10px;
      position: relative;
      .card-text {
        color: white;
        font-weight: 900;
        position: absolute;
        bottom: 0;
        margin-bottom: 50px;
        padding: 0 46px;
        font-size: 25px;
        line-height: 25px;
      }
    }
    .card-container > * {
      z-index:10;
      color: white;
      position: relative;
    }
    .card-one {
      background-image: url('@/assets/img/news-1.jpg');
      background-size: cover;
      height: 363px;
    }
    .card-two {
      background-image: url('@/assets/img/news-2.jpg');
      background-size: cover;
      height: 363px;
    }
    .card-three {
      background-image: url('@/assets/img/news-3.jpg');
      background-size: cover;
      height: 363px;
    }
    .card-container::after{
      content: "";
      width: 100%;
      height: 100%;
      background-color: black;
      position: absolute;
      top: 0;
      left: 0;
      opacity: .4;
      border-radius: 10px;
      z-index: 0;
    }
  }
}

</style>
