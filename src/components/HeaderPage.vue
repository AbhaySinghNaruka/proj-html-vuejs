<template>
  <header>
    <div class="info-bar">
      <div class="info-container">
        <div class="lh left">
          <i class="fa-solid fa-clock"></i>
          Open Hours: Mon - Sat - 9:00 - 18:00
        </div>
        <div class="lh right">
          <div class="phone-number">
            <i class="fa-solid fa-phone"></i>
          {{phoneNumber}}
          </div>
          <div class="email">
            <i class="fa-solid fa-envelope"></i>
            {{email}}
          </div>
          <i class="fa-brands fa-facebook-f lh"></i>
          <i class="fa-brands fa-twitter lh"></i>
          <i class="fab fa-linkedin-in lh"></i>
        </div>
      </div>
    </div>
    <div class="jumbo">
      <div class="jumbo-container">
        <div class="nav">
          <div class="nav-left">
            <span class="blue-arrow">NEX</span><span class="gen">GEN</span>
          </div>

          <div class="nav-right">
            <div class="nav">
              <ul>
                <a href=""><li>HOME</li></a>
                <a href=""><li>SERVICES</li></a>
                <a href=""><li>SKILLS</li></a>
                <a href=""><li>PARTNERS</li></a>
                <li class="btn btn-touch">GET IN TOUCH</li>
              </ul>
            </div>
          </div>
        </div>

        <div class="big-text">
          <div class="content">
            <div class="title">
              Logistics that goes further.
            </div>
            <div class="subtitle">
              For 20 years working with the most innovative in the field of transport.
            </div>
            <div class="btn-container">
              <li class="btn btn-touch">
                GET IN TOUCH
              </li>
              <li class="btn btn-read-more">
                READ MORE
              </li>
            </div>
          </div>
          <div class="blue-behind">
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      phoneNumber: '+1 (305) 1234-5678',
      email: 'hello@example.com',
      address: 'Main Avenue, 987',
    };
  },
};
</script>

<style lang="scss">
  header {
    width: 100%;

    .info-bar {
      background-color: #21333E;
      color: white;
    }

    .info-container {
      width: 61%;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-content: center;
      height: 50px;

      .lh {
        line-height: 50px;
      }

      .right {
        display: flex;
        gap: 40px;
      }
    }

    .jumbo::after{
      content: "";
      display: block;
      width: 100%;
      height: 100%;
      background-color: black;
      position: absolute;
      top: 0;
      left: 0;
      opacity: .5;
      z-index: 0;
    }
    .jumbo > * {
      z-index: 10;
      position: relative;
    }
    .jumbo {
      background-image: url('@/assets/img/jumbo.jpg');
      width: 100%;
      height: 850px;
      background-position-y: -260px;
      background-position-x: -100px;
      background-size: 2250px;
      position: relative;

      .jumbo-container {
        width: 61%;
        margin: 0 auto;
        padding-top: 20px;

        .nav {
          display: flex;
          justify-content: space-between;
        }

        .nav-left {
          padding-top: 10px;
          position: relative;
          span {
            font-weight: 900;
            letter-spacing: 5px;
            font-size: 25px;
            margin-left: 5px;
        }
          .gen {
            color: #C0C3D0;
          }
        }
        .blue-arrow{
          color: #058283;
          background-color: rgba(5, 163, 163, 0.2);
          padding: 15px 0px 15px 35px;
          border-top-left-radius: 100%;
          border-bottom-left-radius: 100%;
        }

        ul{
          display: flex;
          a{
            text-decoration:none;
          }
          li {
            color: white;
            padding: 10px 25px;
          }
          .btn-touch{
            background-color:#05A3A3
          }
          .btn-touch:hover{
            background-color: rgba(5, 130, 131,0.2);
            color: white;
            border: 1px solid #058283;
          }
        }

        .big-text {
          width: 50%;
          margin-left: auto;
          margin-top: 150px;
          color: white;
          position: absolutew;
          transform: scale(.7);
          a{
            text-decoration:none;
          }

          .content {
            position: absolute;
            z-index: 15;

            .title {
            font-size: 110px;
            font-weight:900;
            margin-bottom: 50px;
            line-height: 100px;
            }
            .subtitle {
              font-size: 35px;
            }

            .btn-container {
              display: flex;
              margin-top: 25px;
              gap: 50px;
            }

            .btn-read-more {
              padding: 10px 30px;
              font-size: 25px;
              border: 2px solid #058283;
              color: white;

              a:visited {
                color: white;
              }

            }
            .btn-read-more:hover {
              background-color:#058283;
            }
            .btn-touch {
              padding: 10px 30px;
              font-size: 25px;
              color: white;
              background-color:#058283;
            }
            .btn-touch:hover{
              background-color: rgba(5, 130, 131,0.2);
              color: white;
              border: 1px solid #058283;
            }

          }

          .blue-behind {
            width: 70%;
            height: 45px;
            background-color: #058283;
            z-index: 10;
            position: absolute;
            opacity: .5;
            left: 6px;
            top: 60px;
          }
        }
      }
    }
  }
</style>
