<script>
import AppHeader from './components/AppHeader.vue';
import Content from './components/Content.vue';
import BannerBlu from './components/BannerBlu.vue';

export default{
  name:'App',
  components:{
    AppHeader, 
    Content,
    BannerBlu,
  } 
}
</script>

<template>
  <AppHeader />
  <main>
    <Content/>
    <BannerBlu/>
  </main>
</template>

<style lang="scss"> 
@use './styles/general.scss' as *;

</style>
