<template>
    <body>
        <footer class="container">
            <div class="footer-left">
                <button>
                    SIGN-UP NOW!
                </button>
            </div>
            <div class="footer-right">
                <h5>FOLLOW US</h5>
                <ul>
                    <li v-for="(icon, index) in icons" :key="index">
                        <img :src="require('../assets/img/footer-' + icon.name)"   alt="FB Logo">
                    </li>
                </ul>
            </div>
        </footer>
    </body>
</template>

<script>
export default {
    name: 'FooterBottom',
    data() {
        return {
            icons:
            [
                {
                    name: "facebook.png",
                },
                {
                    name: "twitter.png",
                },
                {
                    name: "youtube.png",
                },
                {
                    name: "pinterest.png",
                },
                {
                    name: "periscope.png"
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
        background-color: #303030;
        padding: 2.1875rem 0;
        footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .footer-left button {
            padding: .75rem;
            background-color: #303030;
            color: #fff;
            border: .1875rem solid $primaryColor;
            font-weight: bold;
        }
        .footer-right {
            display: flex;
            align-items: center;
            ul {
                display: flex;
                li {
                    margin-left: .9375rem;
                }
            }
            h5 {
                color: $primaryColor;
                font-size: 1.3rem;
            }
        }
    }
</style>