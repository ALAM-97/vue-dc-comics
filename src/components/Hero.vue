<template>
    <body>
        <div class="hero">
            
        </div>
    </body>
</template>

<script>
export default {
    name: 'Hero',
}
</script>

<style lang="scss" scoped>
    @import "../../style/common.scss";
    @import "../../style/variables.scss";

    div {
        height: 21.875rem;
        background-image: url("../assets/img/jumbotron.jpg");
        background-position: center top;
        background-size: cover;
    }

</style>