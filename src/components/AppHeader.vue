<script>
export default {
    name: 'AppHeader',
}
</script>


<template> 
    <header>
        <nav>
            <div>
                <img src="../assets/dc-logo.png" alt="logo">
            </div>
            <ul>
                <li><a href="#">CHARACTER</a></li>
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
    nav{
        display: flex;
        justify-content: space-around;
    }
    ul{
        display: flex;
        gap: 1rem;
    }
    li{
       list-style: none;
       
       a{
        text-decoration: none;
        color: rgb(88, 88, 88);
        font-weight: bold;
       }
    }

</style>