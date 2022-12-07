<template>
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
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
.services {
  background-color: #EEF4ED;
  .container {
    width: 1150px;
    margin: 0 auto;
    height: 740px;
    position: relative;
    .services-content {

      width: 100%;
      position: absolute;
      top: 20%;
      display: flex;
      gap: 30px;
      .service{
        width: calc(100% / 3);
      }
      .service-left {
        .logi-title {
          font-weight: 900;
          font-size: 55px;
          line-height: 50px;
          margin: 25px 0;
          color: #21333E;
        }
        .service-left-content {
          font-size: 20px;
          margin-bottom:25px;
          color: #4f5050;
        }
        .tag{
          background-color: #CCE3DE;
          color: #058283;
          padding: 5px 10px;
          margin-right: 15px;
          border-radius: 3px;
        }
        .tag:hover {
          background-color:#058283;
          color: white;
          transition: .3s;
          cursor: pointer;
        }
        .tag:not(:hover){
          background-color:#CCE3DE;
          color:#058283;
          transition: .3s;
        }
        .btn {
          background-color: #058283;
          color: white;
          margin-top: 25px;
          padding: 8px 25px;
        }
        .btn:hover{
          background-color:#CCE3DE;
          color: #058283;
          transition: .3s;
        }
      }
      .service-card{
        padding: 55px 55px 25px 55px;
        background-color: white;
        border-radius: 10px;
        font-size: 19px;
        .service-card-content{
          color: #4f5050;
        }
        h4 {
          font-weight: 900;
          margin: 20px 0;
          color: #21333E;
        }
        .service-img{
          width: 100%;
        }
      }
      .service-card:hover{
        transform: scale(1.1);
        transition: 1s;
        cursor: pointer;
      }
      .service-card:not(:hover){
        transform: scale(1);
        transition: 1s;
      }
    }
  }
}
</style>
