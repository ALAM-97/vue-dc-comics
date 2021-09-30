<template>
    <body>
        <main class="container">
            <ul>
                <li v-for="(service, index) in services" :key="index">
                    <img :class="service.class" :src="service.url" alt="">
                    <h4>{{service.name}}</h4>
                </li>
            </ul>
        </main>
    </body>
</template>

<script>
export default {
    name: "Services",
    data() {
        return {
            services:
        [
            {
                name: "DIGITAL COMICS",
                url: require("../assets/img/buy-comics-digital-comics.png"),
                class: "digital-comics"
            },
            {
                name: "DC MERCHANDISE",
                url:  require("../assets/img/buy-comics-merchandise.png"),
                class: ''
            },
            {
                name: "SUBSCRIPTIONS",
                url: require("../assets/img/buy-comics-subscriptions.png"),
                class: ''
            },
            {
                name: "COMIC SHOP LOCATOR",
                url: require("../assets/img/buy-comics-shop-locator.png"),
                class: "shop-locator"
            },
            {
                name: "DC POWER VISA",
                url: require("../assets/img/buy-dc-power-visa.svg"),
                class: ''
            }
        ]
        }
    }
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