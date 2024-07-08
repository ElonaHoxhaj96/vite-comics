<script>
export default{
  name: 'BannerBlu',
  date(){
    return{

        imgBanner:[
            {
                imgage: '../assets/buy-comics-digital-comics.png',
                testo: 'DIGITAL COMICS'
            },
            {
                imgage: '../assets/buy-comics-merchandise.png',
                testo: 'DC MERCHANDISE'
            },
            {
                imgage: '../assets/buy-comics-subscriptions.png',
                testo:'SUBSCRIPTION'
            },
            {
                imgage: '../assets/buy-comics-shop-locator.png',
                testo: 'COMIC SHOP LOCATOR'
            },
            {
                imgage: '../assets/buy-dc-power-visa.svg',
                testo: 'DC POWER VISA'
            },
    ]

    }
}
}

</script>

<template>
    <section id="bg_blue">
        <div class="cards">
            <div class="images" v-for="(icone, index) in imgBanner" :key="index">
                <img :src="icone.imgage" alt="icona banner">
            </div>
            <div class="testo_img">
                {{icone.testo}}
            </div>
        </div>              
    </section>
</template>

<style lang="scss">
    #bg_blue{
        background-color: rgb(48, 157, 215);
        display: flex;
        height: 150px;
    }
    .cards{
        color: white;
        margin: auto;
        display: flex;
        align-items: center;
        gap: 0.5rem;
  

        .images{
            width: 4rem;

            img{
                width: 100%;
            }
            
        }
    }
</style>