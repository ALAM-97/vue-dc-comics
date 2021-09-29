<template>
  <div id="app">
    <Header/>
    <MainOne/>
    <Services/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import MainOne from './components/MainOne.vue';
import Services from './components/Services.vue';

export default {
  name: 'App',
  components: {
    Header,
    MainOne,
    Services,
  }
}
</script>

<style lang="scss">
  @import "../style/common.scss";
  @import "../style/variables.scss";
  
</style>
