<template>
  <div id="app">
    <Header/>
    <MainOne/>
    <Services/>
    <FooterTop/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import MainOne from './components/MainOne.vue';
import Services from './components/Services.vue';
import FooterTop from './components/FooterTop.vue';

export default {
  name: 'App',
  components: {
    Header,
    MainOne,
    Services,
    FooterTop
  }
}
</script>

<style lang="scss">
  @import "../style/common.scss";
  @import "../style/variables.scss";
  
</style>
