<script>
    export default{
        name: "Cards",
        props: {
            copertina: Object
        }
}
</script>

<template>
    <div class="card_serie">
        <div class="imagine_manifesto">
            <img :src="copertina.thumb" alt="copertina">
        </div>
        <h4>{{copertina.series }}</h4>
    </div>
</template>

<style lang="scss">
@use '../styles/general.scss' as *;
    .card_series{
        width: calc(100% / 6);
        margin: 2rem 0;
        display: flex;
        flex-wrap: wrap;
        justify-content: baseline;
            .imagine_manifesto{
                width: 100%;
                
                    img{
                    width: 100%;
                    height: 100%;
                    }
            }
           
        }
</style>