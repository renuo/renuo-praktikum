<template>
  <div id="app">
    <AboutRenuo/>
  </div>
</template>

<script>
import AboutRenuo from './components/AboutRenuo.vue'

export default {
  name: 'App',
  components: {
    AboutRenuo
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
