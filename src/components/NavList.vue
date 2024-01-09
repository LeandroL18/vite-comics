<script>
    export default{
        name:'NavList',
        data(){
            return{
                links:[
                    {
                        text: "DIGITAL COMICS",
                        url: "#",
                        image: "../img/buy-comics-digital-comics.png",
                    },
                    {
                        text: "DC MERCHANDISE",
                        url: "#",
                        image: "../img/buy-comics-merchandise.png",
                    },
                    {
                        text: "SUBSCRIPTION",
                        url: "#",
                        image: "../img/buy-comics-subscriptions.png",
                    },
                    {
                        text: "COMIC SHOP LOCATOR",
                        url: "#",
                        image: "../img/buy-comics-shop-locator.png",
                    },
                    {
                        text: "DC POWER VISA",
                        url: "#",
                        image: "../img/buy-dc-power-visa.svg",
                    },
                ]

            }
        }
    }
</script>

<template>
    <div>
        <div class="container">
            <ul>
                <li v-for="link in links">
                    <a :href="link.url">
                        <img :src="link.image" alt="img">
                        {{ link.text }}
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    div{
        background-color: rgb(0, 89, 255);
        display: flex;
        align-items: center;
    }

    ul li{
        display: inline-block;
        font-size: 10px;
    }

    li a{
        color: rgb(255, 255, 255);
        font-weight: 800;
        margin-right: -40px;

        &.active, &:hover{
            color: rgb(0, 0, 0);
        }
    }

    img{
        width: 15%;
        vertical-align: -10px;
    }
    
</style>