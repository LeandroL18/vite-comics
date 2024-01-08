<script>
    export default{
        name:'AppHeader'
    }
</script>

<template>
    <header>
        <!-- logo -->
        <div>
            <img src="../img/dc-logo.png" alt="logo">
        </div>
        <!-- nav_bar -->
        <nav>
            <ul>
                <li><a href="#">CHARACTERS</a></li>
                <li><a class="active" href="#">COMICS</a></li>
                <li><a href="#">MOVIES</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">GAMES</a></li>
                <li><a href="#">COLLECTIBLES</a></li>
                <li><a href="#">VIDEOS</a></li>
                <li><a href="#">FANS</a></li>
                <li><a href="#">NEWS</a></li>
                <li><a href="#">SHOP</a></li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    header{
        display:flex;
        align-items: center;
        justify-content: space-around;
        padding: 20px;
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
