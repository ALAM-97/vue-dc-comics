<template>
  <div id="app">
    <Header/>
    <Hero/>
    <MainContent/>
    <Services/>
    <FooterTop/>
    <FooterBottom/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import MainContent from './components/MainContent.vue';
import Services from './components/Services.vue';
import FooterTop from './components/FooterTop.vue';
import FooterBottom from './components/FooterBottom.vue';


export default {
  name: 'App',
  components: {
    Header,
    MainContent,
    Services,
    FooterTop,
    FooterBottom,
    Hero
  }
}
</script>

<style lang="scss">
  @import "../style/common.scss";
  @import "../style/variables.scss";
  
</style>
