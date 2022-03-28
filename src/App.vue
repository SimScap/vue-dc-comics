<template>
  <div id="app">
    <Header/>
    <Banner/>
    <Main/>
    <Foter/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Banner from './components/Banner.vue'
import Main from './components/Main.vue'
import Foter from './components/Foter.vue'


export default {
  name: 'App',
  components: {
    Header,
    Banner,
    Main,
    Foter,
  }
}
</script>

<style lang="scss">
@import "./assets/scss/style.scss";

</style>
