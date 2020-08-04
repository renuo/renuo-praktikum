<template>
  <div id="app">
    <Navigation />
	  <Homepage />
    <Footer />
  </div>
</template>
<script>
// eslint-disable-next-line no-unused-vars
import AboutRenuo from './components/AboutRenuo.vue'
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import Navigation from './components/Navigation.vue'
import Footer from './components/Footer.vue'
import Homepage from './components/Homepage.vue'
import Vue from 'vue'
// Install BootstrapVue
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)
export default {
  name: 'App',
  components: {
    Navigation,
    Homepage,
    Footer
  }
}
</script>

<style lang="scss">
#app {
  font-family: Montserrat, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
}
</style>
