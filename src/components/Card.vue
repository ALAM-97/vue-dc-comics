<template>
    <div class="cards-container">
        <div class="square">
            <img :src="info.thumb" alt="">
            <div>{{info.series.toUpperCase() }}</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: ['info']
}
</script>

<style lang="scss" scoped>
    .square {
        margin: 30px auto;
        height: 170px;
        width: 170px;
        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
        div {
            font-size: 1rem;
            margin-top: 7px;
            color: #fff;
        }
    }
    

</style>