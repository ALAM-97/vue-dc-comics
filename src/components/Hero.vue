<template>
    <body>
        <div class="hero" :style="`background-image: url(${bgImage})`">
            
        </div>
    </body>
</template>

<script>
export default {
    name: 'Hero',
    props: ['bgImage']
}
</script>

<style lang="scss" scoped>
    @import "../../style/common.scss";
    @import "../../style/variables.scss";

    div {
        height: 21.875rem;
        background-position: center top;
        background-size: cover;
    }

</style>                           