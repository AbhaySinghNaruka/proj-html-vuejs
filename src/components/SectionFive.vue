<template>
  <div class="subscribe">
    <div class="container">
        <div class="left col-6">
            <div class="small-text">
                NEWSLETTER
            </div>
            <h1>
                <span class="blue-back">Know</span><span>First</span>
            </h1>
            <div class="left-text">
                <p>
                    Follow closely and receive content about our company
                    and the news of the current market.
                </p>
            </div>
        </div>
        <div class="right col-6">
            <label class="col-12" for="name">
                <input type="text" placeholder="Name"/>
                <input type="text" placeholder="Email"/>
            </label>
            <div class="btn">SUBSCRIBE</div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
    .subscribe {
        background-image: url('@/assets/img/bg-1.jpg');
        height: 450px;
        background-position-y: -300px;
        .container {
            display: flex;
            width: 940px;
            padding: 135px 0;
            gap: 15px;
            .left {
                h1{
                    margin: 35px 0;
                }
                span {
                    font-weight: 900;
                    font-size:50px;
                    color: white;
                };
                .blue-back {
                    padding: 4px 20px;
                    border-radius:5px;
                    background-color: #173338;
                    margin-right: 15px;
                }
                p {
                    font-size: 18px;
                    color: #a3a3a9;
                }
            }
            .right{
                input{
                    width: 100%;
                    padding: 15px 18px;
                    border-radius: 5px;
                    border: none;
                    margin-bottom: 25px;
                    opacity: .5;
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

        }
    }
</style>
