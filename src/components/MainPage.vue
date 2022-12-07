<template>
<main>
    <div class="services">
      <div class="container">
        <div class="services-content">
          <div class="service-left service">
            <div class="small-text">
              OUR BUSINESS AREAS
            </div>
            <h1 class="logi-title">
              Logistics Services
            </h1>
            <div class="service-left-content">
              <p>
                We are leaders in providing logistics services with a set of cutting edge
                technologies and a team of experienced and renowed professionals.
              </p>
            </div>
              <span class="tag">Tradition</span>
              <span class="tag">Quality</span>
              <span class="tag">Security</span>
              <div class="btn">READ MORE</div>
          </div>
          <div class="service-mid service service-card">
            <img class="service-img" src="@/assets/img/gallery-3.jpg" alt="">
            <h4>Technology</h4>
            <div class="service-card-content">
              <p>
                Focused on developing technology solutions adapted to our client's needs.
              </p>
            </div>
          </div>
          <div class="service-right service service-card">
            <img class="service-img" src="@/assets/img/gallery-5.jpg" alt="">
            <h4>Transport</h4>
            <div class="service-card-content">
              <p>
                We develop operational strategies to imrpove logistical efficiency
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
</main>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>

main {
  height: 4500px;

  .services {
    background-color: #EEF4ED;
    .container {
      width: 1150px;
      margin: 0 auto;
      height: 740px;
      position: relative;
      .services-content {
        height: 55%;
        width: 100%;
        position: absolute;
        top: 20%;
        display: flex;
        gap: 30px;
        .service{
          width: calc(100% / 3);
        }
        .service-left {
          .small-text {
            font-size: small;
            font-weight: 900;
            color: #00A6A6;
          }
          .logi-title {
            font-weight: 900;
            font-size: 55px;
            line-height: 50px;
            margin: 25px 0;
          }
          .service-left-content {
            font-size: 20px;
            margin-bottom:25px
          }
          .tag{
            background-color: #CCE3DE;
            color: #058283;
            padding: 5px 10px;
            margin-right: 15px;
            border-radius: 3px;
          }
          .btn {
            background-color: #058283;
            color: white;
            margin-top: 25px;
            padding: 8px 25px;
          }
        }
        .service-card{
          padding: 50px;
          background-color: white;
          border-radius: 10px;
          font-size: 19px;
          h4 {
            font-weight: 900;
            margin: 20px 0;
          }
          .service-img{
            width: 100%;
          }
        }
      }
    }
  }

}

</style>
