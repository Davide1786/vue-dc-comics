<template>
  <div id="app">
    <Header />
    <MainTop />
    <Main />
    <MainBottom />
    <FooterTop />
    <FooterB />

 



  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainTop from './components/MainTop.vue'
import Main from './components/Main.vue'
import MainBottom from './components/MainBottom.vue'
import FooterTop from './components/FooterTop.vue'
import FooterB from './components/FooterB.vue'





export default {
  name: 'App',
  components: {
    Header,
    MainTop,
    Main,
    MainBottom,
    FooterTop,
    FooterB,


  }
}
</script>

<style lang="scss">
  @import './components/Style/Common';
 
</style>
