<script>
export default{
  name: 'BannerBlu',
  data() {
    return {
        activeIcona: 0,
        imgBanner: [
            {
                imgage: 'src/assets/buy-comics-digital-comics.png',
                testo: 'DIGITAL COMICS'
            },
            {
                imgage: 'src/assets/buy-comics-merchandise.png',
                testo: 'DC MERCHANDISE'
            },
            {
                imgage: 'src/assets/buy-comics-subscriptions.png',
                testo:'SUBSCRIPTION'
            },
            {
                imgage: 'src/assets/buy-comics-shop-locator.png',
                testo: 'COMIC SHOP LOCATOR'
            },
            {
                imgage: 'src/assets/buy-dc-power-visa.svg',
                testo: 'DC POWER VISA'
            },
        ], 
        methods: {
            iconaAttiva(index) {
            this.activeIcona = index;
            console.log(this.iconaAttiva);
        }
        }
    }
}
}
</script>

<template>
    <section id="bg_blue">
        <ul class="ds_flex">
            <li class="ds_flex" v-for="(icona, index) in imgBanner" :key="index">
                <a href="#" class="ds_flex" >
                    <div class="images">
                        <img :src="icona.imgage" alt="icona banner">
                    </div>
                    <span class="testo_img">{{ icona.testo }}</span>
                </a>
            </li>
        </ul>
                     
    </section>
</template>

<style lang="scss">
    @use '../styles/general.scss' as *;
    #bg_blue{
        background-color: #0282f9;
        display: flex;
        height: 150px;
    }
    .ds_flex{
        color: white;
        margin: auto;
        display: flex;
        align-items: center;
        gap: 1rem;
  
        a{
            gap: 0.3rem;
        }
        .images{
            width: 3.5rem;

            img{
                width: 100%;
            }
            
        }
    }
</style>