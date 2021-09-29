<template>
  <div id="app">
    <Header/>
    <MainOne/>
    <Services/>
    <FooterTop/>
    <FooterBottom/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import MainOne from './components/MainOne.vue';
import Services from './components/Services.vue';
import FooterTop from './components/FooterTop.vue';
import FooterBottom from './components/FooterBottom.vue';

export default {
  name: 'App',
  components: {
    Header,
    MainOne,
    Services,
    FooterTop,
    FooterBottom
  }
}
</script>

<style lang="scss">
  @import "../style/common.scss";
  @import "../style/variables.scss";
  
</style>
