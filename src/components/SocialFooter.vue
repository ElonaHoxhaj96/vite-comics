<script>
export default{
    name:'SocialFooter',
    data() {
        return{
        socialIconas: [
        'src/assets/footer-facebook.png',
        'src/assets/footer-twitter.png',
        'src/assets/footer-pinterest.png',
        'src/assets/footer-periscope.png' 
    ]
        }
    }
  
   
}
</script>

<template>
    <section id="container_social">
        <button>SIGN-UN NOW</button>
        <div id="icone_social">
            <a href="#" class="blu">FOLLOW US</a>
            <a href="#" v-for="(icon, index) in socialIconas" :key="index">
                <img :src="icon" alt="">
            </a>
        </div>
    </section>
    
</template>

<style lang="scss"> 
    @use '../styles/general.scss' as *;
    #container_social{
        background-color: #303030;
        height: 60px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        
            #icone_social{
            display: flex;
            align-items: center;
            gap: 0.5rem;
            margin-right: 11rem;
                img{
                filter: invert(1);
                }
            }
    }
    button{
        margin-left: 11rem;
        color: white;
        background-color: #303030;
        border: solid #0282f9;
        padding: 0.5rem;
    }

</style>
