<script>
    export default{
        name:'AppHeader',
        data(){
            return{
                links:[
                    {
                        text: "CHARACTERS",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "COMICS",
                        url: "#",
                        current: true,
                    },
                    {
                        text: "MOVIES",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "TV",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "GAMES",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "COLLECTIBLES",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "VIDEOS",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "FANS",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "NEWS",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "SHOP",
                        url: "#",
                        current: false,
                    }
                ]
            }
        }
    }
</script>

<template>
    <header>
        <div class="container">
            <!-- logo -->
            <div>
                <img src="../assets/dc-logo.png" alt="logo">
            </div>
            <!-- navigazione principale -->
            <nav>
                <ul>
                    <li v-for="(link,i) in links" :key="i">
                        <a :href="link.url" :class="link.current ? 'active' : ''">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;
    .container{
        display:flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px;
    }
    img{
        width: 70%;
    }
    nav ul li{
        display: inline-block;
        margin: 0 8px 10px 8px;
        font-size: 12px;
    }
    li a{
        color: rgb(0, 0, 0);
        font-weight: 800;

        &.active, &:hover{
            color: blue;
        }
    }
</style>
