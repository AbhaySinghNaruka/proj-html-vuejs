<template>
  <footer>
    <div class="infos">
        <div class="container">
            <div class="column">
                <div class="name">
                    <span class="blue-arrow">NEX</span><span class="gen">GEN</span>
                </div>
                <p>
                    A Functional HTML Template for Corporate & Business
                </p>
                <div class="contact">
                    <div class="contact-row">
                        <i class="fa-solid fa-phone"></i><span>+1 (305) 1234-5678</span>
                    </div>
                    <div class="contact-row">
                        <i class="fa-solid fa-envelope"></i><span>hello@example.com</span>
                    </div>
                    <div class="contact-row">
                        <i class="gps fa-solid fa-location-dot"></i><span>Main Avenue, 987</span>
                    </div>
                    <div class="btn btn-footer">
                        GET IN TOUCH
                    </div>
                </div>
            </div>
            <div class="column links">
                <div class="title">
                    <h4>About</h4>
                    <ul>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            The Company
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Institutional
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Social & Events
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Innovation
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Enviroment
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Technology
                        </li>
                    </ul>
                </div>
            </div>
            <div class="column links">
                <div class="title">
                    <h4>Transport</h4>
                    <ul>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Industrialized
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Chemicals
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Packaged Liquids
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Construcion
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Laminated Wood
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            And others
                        </li>
                    </ul>
                </div>
            </div>
            <div class="column links">
                <div class="title">
                    <h4>Support</h4>
                    <ul>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Responsibility
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Terms of Use
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            About Cookies
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Privacy Policy
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Accessibility
                        </li>
                        <li><i class="fa-solid fa-chevron-right"></i>
                            Information
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
    <div class="copyright">
        <div class="footer-container">
            <div class="left">
                Enjoy the low price. We are tracking any intention of piracy.
            </div>
            <div class="right">
                &#169;2020 NEXGEN is Proudly Powerewd by <span><a href="">Codings</a></span>.
            </div>
        </div>

    </div>
</footer>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
    .infos {
        height: 640px;
        background-image: url('@/assets/img/bg-10.jpg');
        background-position-y: -220px;
        padding: 125px 0;
        .container{
            width: 1120px;
            height: 100%;

            display: flex;
            justify-content: space-between;
            gap: 15px;
            .links {
                background-color: rgba(175, 175, 175, 0.05);
                padding: 50px 45px;
                border-radius: 10px;
            }
            .column {
                width: calc(100%/4);
                p{
                    color:#adadaf;
                }
                h4{
                    color: white;
                    font-weight: 900;
                    margin-bottom: 25px;
                }
                ul {
                    padding-left: 0;
                    li {
                        color: #adadaf;
                        margin-bottom: 10px;
                        font-size: 18px;
                    }
                }

                .name{
                    margin-bottom: 25px;
                    span {
                        font-weight: 900;
                        letter-spacing: 5px;
                        font-size: 25px;
                        margin-left: 5px;
                    }
                    .gen {
                        color: #C0C3D0;
                      }
                    .blue-arrow{
                      color: #05A3A3;
                      background-color: rgba(5, 163, 163, 0.2);
                      padding: 15px 0px 15px 35px;
                      border-top-left-radius: 100%;
                      border-bottom-left-radius: 100%;
                    }
                }
                .contact{
                    .contact-row {
                        margin-bottom: 25px;
                        font-size: 20px;
                        color: #adadaf;
                        i {
                            margin-right: 15px;
                        }
                    }
                    .btn-footer {
                        color: white;
                        border: 1px solid #058283;
                        margin-top: 25px;
                        padding: 8px 25px;
                    }
                    .btn-footer:hover{
                        background-color:#058283;
                        transition: .3s;
                    }
                }

            }
        }
    }
    .copyright{
        background-color: #0D0D11;
        color: #adadaf;

        .footer-container{
            width: 1120px;
            margin: 0 auto;
            height: 60px;
            display: flex;
            justify-content: space-between;
            position: relative;
            .right{
                position: absolute;
                bottom: 0px;
                right: 0;
            }
            .left{
                position: absolute;
                bottom: 0px;

            }
            a{
                text-decoration: none;
            }
            a:visited{
                color: #058283
            }
        }

    }
</style>
