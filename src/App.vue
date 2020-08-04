<template>
  <div id="app">
    <AboutRenuo/>
  </div>
</template>

<script>
import AboutRenuo from './components/AboutRenuo.vue'
// eslint-disable-next-line no-unused-vars
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

export default {
  name: 'App',
  components: {
    AboutRenuo
  }
}
</script>

<style lang="scss">
#app {
  font-family: Montserrat, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
