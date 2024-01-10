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
            <div class="container">
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
            <div class="container">
                <div>
                    <a id="sign" href="#">SIGN-UP NOW!</a>
                </div>

                <div>
                    <span>FOLLOW US</span>
                    <font-awesome-icon :icon="['fab', 'facebook']" />
                    <font-awesome-icon :icon="['fab', 'twitter']" />
                    <font-awesome-icon :icon="['fab', 'youtube']" />
                    <font-awesome-icon :icon="['fas', 'location-dot']" />
                    <font-awesome-icon :icon="['fas', 'location-dot']" />
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
    .container:first-child{
        display: flex;
        padding-top: 15px;
    }

    .container:last-of-type{
        padding: 15px;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    div:last-child{
        margin-top: -15px;
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
    }

    ul{
        margin-top: 10px;
    }

    img{
        width: 55%;
    }

    #bg_grey{
        background-color: rgb(80, 80, 80);
    }
    
</style>