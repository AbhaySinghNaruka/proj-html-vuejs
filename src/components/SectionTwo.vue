<template>
  <div class="the-company">
    <div class="left col-6">
      <div class="container col-7">
        <div class="top">
          <div class="small-text">
            ABOUT THE NETWORK
          </div>
          <div class="title">
            <h1><span class="back-color">The</span>Company</h1>
          </div>
          <div class="content">
            <p>
              With all of this expertise and capability comes
              an unrivalled commitment to cusotmer service
            </p>
          </div>
        </div>
        <div class="bottom">
          <div class="percent-section">
            <div class="percent-number">
              0<span class="pedice">%</span>
            </div>
            <div class="text">
              <h4 class="percent-title">Leadership</h4>
              <div class="percent-content">
                Lorem ipsum dolor sit amet consectetur adipiscing elit.
              </div>
            </div>
          </div>
          <div class="percent-section">
            <div class="percent-number">
              0<span class="pedice">%</span>
            </div>
            <div class="text">
              <h4 class="percent-title">Psychology</h4>
              <div class="percent-content">
                Lorem ipsum dolor sit amet consectetur adipiscing elit.
              </div>
            </div>
          </div>
          <div class="percent-section">
            <div class="percent-number">
              1<span class="pedice">%</span>
            </div>
            <div class="text">
              <h4 class="percent-title">Flexibility</h4>
              <div class="percent-content">
                Lorem ipsum dolor sit amet consectetur adipiscing elit.
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="right col-6"></div>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
  .the-company {
    height: 1000px;
    display: flex;
    .left {
      background-color: #111117;
      height: 1000px;
    }
    .right{
      background-image: url('@/assets/img/about-5.jpg');
      background-repeat: no-repeat;
      background-size: cover;
    }
    .container{
      height: 100%;
      margin-right: 0;
      padding: 130px 75px 0px 0px;
      .top {
        margin-bottom: 75px;
          h1 {
          font-weight: 900;
          font-size: 55px;
          color: white;
          margin: 25px 0;
        }
        .content {
          color: #919194;
          font-size: 17px;
        }
      }
      .bottom{
        .percent-section {
          display: flex;
          margin: 75px 0;
          .percent-number {
            font-size: 30px;
            font-weight: 900;
            padding: 20px;
            min-width: 100px;
            height: 100px;
            text-align: center;
            border-radius: 100%;
            border: 10px solid #232328;
            transform: scale(1.1);
            color: #919194;
            margin-right: 25px;
            .pedice {
              font-size: 15px;
            }
          }
          h4 {
            font-weight: 900;
            color: white;
          }
          .percent-content {
            font-size: 19px;
            color: #919194;
          }
        }
      }
    }
  }
</style>
