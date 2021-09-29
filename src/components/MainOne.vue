<template>
    <body>
        <main class="container">
            <h2> --> Content goes here </h2>
        </main>
    </body>
</template>

<script>
export default {
    name:' MainOne',
}
</script>

<style lang="scss" scoped>
    @import "../../style/common.scss";
    @import "../../style/variables.scss";

    body {
        background-color: $darkColor;
        h2 {
            color: #fff;
            padding: 50px 0;
        }
    }
</style>