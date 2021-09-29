<template>
  <div id="app">
    <Header/>
    <MainOne/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import MainOne from './components/MainOne.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainOne
  }
}
</script>

<style lang="scss">
  @import "../style/common.scss";
  @import "../style/variables.scss";
  
</style>
