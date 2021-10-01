<template>
    <body>
        <main class="container">
            <div class="section-header">
                CURRENT SERIES
            </div>
            <div class="cards">
                <Card class="single-card" v-for="(data, index) in myJson" :key="index" :info="data"/>
            </div>
            <div class="section-footer">
                LOAD MORE
            </div>
        </main>
    </body>
</template>

<script>
    import json from "./dc-comics.json";
    import Card from "./Card.vue";

    export default {
        name: 'CurrentSeries',
        data() {
            return {
                myJson: json  
            }
        },
        components: {
            Card
        }
    }
</script>

<style lang="scss" scoped>
    @import "../../style/common.scss";
    @import "../../style/variables.scss";

    body {
        background-color: $darkColor;
        .container {
            position: relative;
            .section-header {
                color: #fff;
                font-size: 1.8rem;
                font-weight: bold;
                padding: 10px 20px;
                background-color: $primaryColor;
                position: absolute;
                top: -30px;
                left: -20px;
            }
            .section-footer {
                color: #fff;
                font-size: 1.4rem;
                font-weight: bold;
                padding: 10px 70px;
                background-color: $primaryColor;
                position: absolute;
                left: 50%;
                bottom: 30px;
                transform: translateX(-50%);
            }
        }
        
    }
    .cards {
        display: flex;
        flex-wrap: wrap;
        padding: 30px 0 140px 0;
        .single-card {
            width: calc(100% / 6);
        }
    }
</style>