<script>
import AppHeader from './AppHeader.vue';

    export default{
    name: 'AppFooter',
    components: { AppHeader }
}
</script>

<template>
    <!-- Footer up -->
    <section>
        <div id="bg">
            <div id="container_up" class="container">
                <div>
                    DC COMICS
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>      
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul> <br>

                    SHOP
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>

                <div>
                    DC
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contacts Us</a></li>
                    </ul>
                </div>

                <div>
                    SITES
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
                

                <div>
                    <img src="../assets/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
    </section>

    <!-- Footer down -->
    <section>
        <div id="bg_grey">
            <div id="container_down" class="container">
                <div>
                    <a id="sign" href="#">SIGN-UP NOW!</a>
                </div>

                <div>
                    <span>FOLLOW US</span>
                    <i class="fa-brands fa-facebook"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-youtube"></i>
                    <i class="fa-brands fa-pinterest-p"></i>
                    <i class="fa-solid fa-location-dot"></i>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    #bg{
        background-image: url("../assets/footer-bg.jpg");
        color: white;
    }
    #container_up{
        display: flex;
        padding: 30px;
    }

    #container_down{
        padding: 30px;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    a{
        color: grey;
    }
    
    #sign{
        color: white;
        border: 2px solid rgb(0, 89, 255);
        padding: 10px;
    }

    span{
        color: rgb(0, 89, 255);
        font-weight: bold;
        vertical-align: -15px;
        margin-right: 20px;
    }

    ul{
        margin-top: 10px;
    }

    img{
        width: 66%;
        margin: -30px 0px;
    }

    #bg_grey{
        background-color: rgb(80, 80, 80);
    }
    
    .fa-facebook{
        vertical-align: -22px;
        margin-right: 10px;
        font-size: 25px;
        color: rgb(80, 80, 80);
        background-color: grey;
        padding: 3px;
        border-radius: 50%;
    }

    .fa-twitter{
        vertical-align: -22px;
        margin-right: 10px;
        font-size: 25px;
        color: rgb(80, 80, 80);
        background-color: grey;
        padding: 3px;
        border-radius: 50%;
    }

    .fa-pinterest-p{
        vertical-align: -22px;
        margin-right: 10px;
        font-size: 25px;
        color: rgb(80, 80, 80);
        background-color: grey;
        padding: 3px 7px;
        border-radius: 50%;
    }

    .fa-youtube{
        vertical-align: -22px;
        margin-right: 10px;
        font-size: 25px;
        color: rgb(80, 80, 80);
        background-color: grey;
        padding: 3px;
        border-radius: 50%;
    }
    .fa-location-dot{
        vertical-align: -22px;
        margin-right: 10px;
        font-size: 25px;
        color: rgb(80, 80, 80);
        background-color: grey;
        padding: 3px 6.5px;
        border-radius: 50%;
    }

</style>