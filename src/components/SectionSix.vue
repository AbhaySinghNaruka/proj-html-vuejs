<template>
    <div class="form-section">
        <div class="container">
            <div class="left">
                <div class="small-text">
                    <span>SEND A MESSAGE</span>
                </div>
                <h1>Get in <span>Touch</span></h1>
                <p>We will respond to your message as soon as possible.</p>
                <form action="">
                    <div class="row">
                        <div class="col">
                            <input type="text"
                            class="form-control my-form-control"
                            placeholder="Name"
                            aria-label="First name">
                        </div>
                        <div class="col">
                            <input type="text"
                            class="form-control my-form-control"
                            placeholder="Email"
                            aria-label="Last name">
                        </div>
                    </div>
                    <div class="row">
                        <div class="col">
                            <input type="text"
                            class="form-control my-form-control"
                            placeholder="Phone"
                            aria-label="First name">
                        </div>
                        <div class="col">
                            <!-- eslint-disable -->
                            <select class="form-select form-control my-form-control"
                                    name="infos"
                                    id="infos">
                                <option value="more-infos">
                                    More Infos
                                </option>
                            </select>

                        </div>
                    </div>
                    <div class="row">
                        <div class="col">
                            <textarea class="form-control my-form-control"
                            name="message"
                            id="message"
                            cols="100"
                            rows="7"
                            placeholder="Message">
                        </textarea>
                        </div>
                    </div>
                    <div class="btn btn-left">SEND</div>
                </form>
            </div>

            <div class="right">
                <div class="text">
                    <h3>Example Inc.</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    <p>Praesent diam lacus, dapibus sed imperediet consectetur.</p>
                </div>
                <div class="contact">
                    <div class="contact-row">
                        <i class="fa-solid fa-phone"></i><span> +1 (305) 1234-5678</span>
                    </div>
                    <div class="contact-row">
                        <i class="fa-solid fa-envelope"></i><span>hello@example.com</span>
                    </div>
                    <div class="contact-row">
                        <i class="gps fa-solid fa-location-dot"></i><span>Main Avenue, 987</span>
                    </div>
                    <div class="btn btn-right">
                        VIEW MAP
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
.form-section{
    background-color: #EEF4ED;
    .container{
        width: 1120px;
        height: 750px;
        padding: 125px 0;
        display: flex;
        .left{
            width: 60%;
            height: 500px;
            h1{
                font-weight: 900;
                font-size:50px;
                margin: 15px 0;
                span {
                    background-color:#CCE3DE;
                    color: #058283;
                    padding: 4px 20px;
                    border-radius:5px;
                }
            }
            p{
                margin-bottom: 50px;
            }
            .my-form-control {
                margin-bottom: 15px;
                border-radius: 3px;
                padding: 10px 15px;
                background-color:#DCE2DB;
            }
            #infos {
                color: rgb(108, 108, 108);
            }
            .btn-left {
                background-color: #058283;
                color: white;
                margin-top: 25px;
                padding: 8px 25px;
            }
            .btn-left:hover{
                background-color:#CCE3DE;
                color: #058283;
                transition: .3s;
            }

        }
        .right {
            width: 40%;
            height: 500px;
            padding: 0 40px;
            h3{
                font-weight: 800;
            }
            .contact-row {
                display: flex;
                align-items: center;
                margin-bottom: 15px;
                i{
                    margin-right: 20px;
                    background-color: #CCE3DE;
                    padding: 15px;
                    border-radius: 100%;
                    color: #058283;
                    font-size: 20px;
                }
                .gps {
                    padding: 15px 17px;
                }
                span {
                    color: #058283;
                    font-size: 20px;
                }
            }
            .btn-right {
                color: #058283;
                border: 1px solid #058283;
                margin-top: 25px;
                padding: 8px 25px;
            }
            .btn-right:hover{
                background-color:#058283;
                color: white;
                transition: .3s;
            }
        }
    }
}

</style>
