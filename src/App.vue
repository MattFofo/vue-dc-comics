<template>
  <div id="app">
        <HeaderDC />
        <mainDC />
  </div>
</template>

<script>
import HeaderDC from './components/HeaderDC.vue'
import mainDC from './components/mainDC.vue'

export default {
  name: 'App',
  components: {
    HeaderDC,
    mainDC
  }
}
</script>

<style lang="scss">
@import './assets/styles/style.scss';
</style>
