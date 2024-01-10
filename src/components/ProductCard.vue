<script>
    export default{
        name:'ProductCard',
        props:{
            details: Object
        }
    }
</script>

<template>
    <div id="card">
        <img :src="details.thumb" alt="img">
        <h6>{{ details.series }}</h6>
    </div>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    #card{
        width: calc((100% / 6) - 15px);
    }

    img{
        width: 100%;
        height: 100px;
    }

    h6{
        color: rgb(255, 255, 255);
    }
    
</style>