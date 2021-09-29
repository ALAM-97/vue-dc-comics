<template>
    <body>
        <footer class="container">
            <div class="footer-left">
                <div class="col">
                    <h6>DC COMICS</h6>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h6>SHOP</h6>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="col">
                    <h6>DC</h6>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="col">
                    <h6>SITES</h6>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
            <div class="footer-right">
                <img src="../assets/dc-logo-bg.png" alt="Footer DC Logo">
            </div>
        </footer>
    </body>
</template>

<script>
export default {
    name: 'FooterTop'
}
</script>

<style lang="scss" scoped>
    @import "../../style/common.scss";
    @import "../../style/variables.scss";

    body {
        background-image: url("../assets/footer-bg.jpg");
        background-size: cover;
        footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-height: 22.75rem;
            overflow: hidden;
        }
        .footer-left {
                display: flex;
                .col {
                    margin-right: 40px;
                    h6 {
                        color: #fff;
                        font-size: 1.1rem;
                        margin-bottom: .75rem;
                    }
                    & ul {
                            color: #fff;
                            opacity: .6;
                            font-size: .9rem;
                            li {
                                margin-bottom: .1875rem;
                                &:last-child {
                                    margin-bottom: .75rem;
                                }
                            }
                        }
                }
        }
        .footer-right {
            display: flex;
            img {
                margin-left: auto;
                width: 80%;
            }
        }
    }

</style>