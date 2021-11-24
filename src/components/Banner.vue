<template>
    <section>
        <div class="container">
            <div>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>digital comics</span>
            </div>
            <div>
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                <span>dc merchandise</span>
            </div>
            <div>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                <span>subscription</span>
            </div>
            <div>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <span>comic shop locator</span>
            </div>
            <div>
                <img class="smaller" src="../assets/img/buy-dc-power-visa.svg" alt="">
                <span>dc power visa</span>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'Banner',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    section {
        
        background-color: #0282f9;

        .container {

            display: flex;
            justify-content: space-around;
            align-items: center;
            height: 200px;
            
            div {
                width: 15%;
                display: flex;
                justify-content: center;
                align-items: center;

                img {
                    height: 70px;
                }
                img.smaller {
                    height: 50px;
                }

                span {
                    text-transform: uppercase;
                    color: white;
                    margin-left: 10px;
                }
            }
        }
    }
</style>