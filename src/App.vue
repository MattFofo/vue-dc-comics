<template>
  <div id="app">
        <HeaderDC />
        <MainDC />
        <FooterDC />
  </div>
</template>

<script>
import HeaderDC from './components/HeaderDC.vue'
import MainDC from './components/MainDC'
import FooterDC from './components/FooterDC'

export default {
  name: 'App',
  components: {
    HeaderDC,
    MainDC,
    FooterDC
  }
}
</script>

<style lang="scss">
@import './assets/styles/style.scss';
</style>
