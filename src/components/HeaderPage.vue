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
            <span class="nex">NEX</span>
          </div>

          <div class="nav-right">
            <div class="nav">
              <ul>
                <li
                  v-for="(link,i) in menuLinks"
                  :key="i"
                  :class="(link.isActive)? 'active-link' : ''"
                >
                  <a
                    href="#"
                    @click="activateLink(i)"
                  >{{ link.label.toUpperCase() }}</a>
                </li>
              </ul>
            </div>
          </div>
        </div>

        <div class="get-in-touch">
          <div class="content">
            <div class="title">
              Logistics that goes further.
            </div>
            <div class="subtitle">
              For 20 years working with the most innovative in the field of transport.
            </div>
            <div class="btn-container">
              <li class="btn"
              v-for="(link,i) in titleLinks"
              :key="i"
              :class="(link.isActive)? 'active-link' : ''"
            >
              <a
                href="#"
                @click="activateLink(i)"
              >{{ link.label.toUpperCase() }}</a>
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
  methods: {
    activateLink(index) {
      this.menuLinks.forEach((link) => {
        /* eslint-disable */
        link.isActive = false;
      });
      this.menuLinks[index].isActive = true;
    },
    activateLink(index) {
      this.titleLinks.forEach((link) => {
        /* eslint-disable */
        link.isActive = false;
      });
      this.titleLinks[index].isActive = true;
    },
  },
  data() {
    return {
      phoneNumber: '+1 (305) 1234-5678',
      email: 'hello@example.com',
      address: 'Main Avenue, 987',

      menuLinks: [
        {
          label: 'home',
          isActive: false,
          index: 0,
        },
        {
          label: 'services',
          isActive: false,
        },
        {
          label: 'skills',
          isActive: false,
        },
        {
          label: 'partners',
          isActive: false,
        },
        {
          label: 'blog',
          isActive: false,
        },
        {
          label: 'get in touch',
          isActive: true,
        },
      ],
      titleLinks: [
        {
          label: 'get in touch',
          isActive: true,
        },
        {
          label: 'read more',
          isActive: false
        }
      ]
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

    .jumbo {
      background-image: url('@/assets/img/jumbo.jpg');
      width: 100%;
      height: 850px;
      background-position-y: -260px;
      background-position-x: -100px;
      background-size: 2250px;

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
            font-size: 18px;
            margin-left: 5px;
          }
          .gen {
            color: #C0C3D0;
          }
          .nex {
            position: relative;
            right: 120px;
            color: #05A3A3;
          }
        }
        .blue-arrow{
          color: #05A3A3;
          background-color: #05A3A3;
          opacity: 30%;
          padding: 15px 0px 15px 35px;
          border-top-left-radius: 100%;
          border-bottom-left-radius: 100%;
        }

        ul{
          display: flex;
          li {
            padding: 10px 25px;
            a:visited {
              color: white;
            }

            &.active-link {
              background-color: #058283;
            }
          }
        }

        .get-in-touch {
          width: 50%;
          margin-left: auto;
          margin-top: 150px;
          color: white;
          position: absolutew;
          transform: scale(.7);

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
              justify-content: flex-end;
              margin-top: 25px;
              gap: 50px;
            }

            .btn {
              padding: 10px 30px;
              font-size: 25px;
              border: 2px solid #058283;

            a:visited {
              color: white;
            }

            &.active-link {
              background-color: #058283;
            }
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
