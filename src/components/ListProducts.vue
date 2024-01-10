<script>
import ProductCard from './ProductCard.vue'


    export default{
        name:'ListProducts',
        components:{
            ProductCard
        }
    }
</script>

<template>
    <div id="jumbotron">
        <span>CURRENT SERIES</span>
    </div>

    <div id="bg_black">
        <div class="container">
            <ProductCard/>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    #jumbotron{
        width: 100%;
        height: 230px;
        background-image: url(../assets/jumbotron.jpg);
        background-size: cover;
        position: relative;
    }
    #jumbotron span{
        color: white;
        font-weight: bold;
        font-size: 18px;
        background-color: rgb(0, 89, 255);
        padding: 7px;
        position: absolute;
        bottom: -18px;
        left: 200px;
    }

    #bg_black{
        background-color: black;
        padding: 30px 0;
    }
    h1{
        color: rgb(255, 255, 255);
        text-align: center;
    }
    
</style>