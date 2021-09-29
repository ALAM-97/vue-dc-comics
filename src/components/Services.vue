<template>
    <body>
        <main class="container">
            <ul>
                <li>
                    <img class="digital-comics" src="../assets/buy-comics-digital-comics.png" alt="">
                    <h4>DIGITAL COMICS</h4>
                </li>
                <li>
                    <img src="../assets/buy-comics-merchandise.png" alt="">
                    <h4>DC MERCHANDISE</h4>
                </li>
                <li>
                    <img src="../assets/buy-comics-subscriptions.png" alt="">
                    <h4>SUBSCRIPTION</h4>
                </li>
                <li>
                    <img class="shop-locator" src="../assets/buy-comics-shop-locator.png" alt="">
                    <h4>COMIC SHOP LOCATOR</h4>
                </li>
                <li>
                    <img src="../assets/buy-dc-power-visa.svg" alt="">
                    <h4>DC POWER VISA</h4>
                </li>
            </ul>
        </main>
    </body>
</template>

<script>
export default {
    name: "Services",
}
</script>
    
<style lang="scss" scoped>
    @import "../../style/common.scss";
    @import "../../style/variables.scss";

    body {
        background-color: $primaryColor;
        main.container {
            padding: 40px 0;
            ul {
                display: flex;
                justify-content: space-around;
                li {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    width: calc(100% / 5);
                    img {
                        width: 25%;
                        margin-right: 10px;
                        &.shop-locator {
                            width: 18%;
                        }
                        &.digital-comics {
                            width: 22%;
                        }
                    }
                    h4 {
                        color: #fff;
                    }
                }
            }
            
        }
    }
</style>