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

            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    #bg{
        background-image: url("../assets/footer-bg.jpg");
    }
    .container{
        display: flex;
        justify-content: space-between;
    }
    img{
        width: 55%;
    }

    
</style>