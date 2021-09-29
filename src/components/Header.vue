<template>
    <body>
        <header class="container">
            <img src="../assets/dc-logo.png" alt="DC Logo">
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index"><a :href="link.url" :class="{ active : link.current }">{{link.title}}</a></li>
                </ul>
            </nav>
        </header>
    </body>
    
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            links: 
            [
                {
                    title: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                {
                    title: 'COMICS',
                    url: '#',
                    current: true
                },
                {
                    title: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    title: 'TV',
                    url: '#',
                    current: false
                },
                {
                    title: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    title: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    title: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    title: 'FANS',
                    url: '#',
                    current: false
                },
                {
                    title: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    title: 'SHOP',
                    url: '#',
                    current: false
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "../../style/common.scss";
    @import "../../style/variables.scss";

    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        img {
            width: 8%;
        }
        ul {
            display: flex;
            li {
                list-style: none;
                a {
                    display: flex;
                    line-height: 110px;
                    text-decoration: none;
                    display: inline-block;
                    margin-left: 20px;
                    color: $darkColor;
                    &.active {
                        color: $primaryColor;
                        border-bottom: 4px solid $primaryColor;
                    }
                }
            }
        }
    }
</style>