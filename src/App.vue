<template>
  <div id="app">
    <Header/>
    <Banner/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Banner from './components/Banner.vue'

export default {
  name: 'App',
  components: {
    Header,
    Banner
  }
}
</script>

<style lang="scss">
@import "./assets/scss/style.scss";

</style>
