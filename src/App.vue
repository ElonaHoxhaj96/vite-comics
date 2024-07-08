<script>
import AppHeader from './components/AppHeader.vue';
import Content from './components/Content.vue';
import BannerBlu from './components/BannerBlu.vue';
import LinkFooter from './components/LinkFooter.vue';
import SocialFooter from './components/SocialFooter.vue'

export default{
  name:'App',
  components:{
    AppHeader, 
    Content,
    BannerBlu,
    LinkFooter,
    SocialFooter 
  } 
}
</script>

<template>
  <AppHeader />
  <main>
    <Content/>
    <BannerBlu/>
  </main>
  <footer>
    <LinkFooter/>
    <SocialFooter/>
  </footer>
</template>

<style lang="scss"> 
@use './styles/general.scss' as *;

</style>
