<template>
  <div id="app">
    <Navigation @selected="setActive"/>
      <div v-show="isActive('home')">
    <Homepage />
      </div>
      <div v-show="isActive('renuo')">
        <HelloWorld />
      </div>
    <Footer />
  </div>
</template>
<script>
import Navigation from './components/Navigation.vue'
import Footer from './components/Footer.vue'
import Homepage from './components/Homepage.vue'
import HelloWorld from './components/HelloWorld.vue'
import Vue from 'vue'
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
// Install BootstrapVue
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)
export default {
  name: 'App',
  data () {
    return {
      activeBody: 'home' // visible to template
    }
  },
  methods: {
    isActive (menuItem) {
      return this.activeBody === menuItem
    },
    setActive (menuItem) {
      console.log('Test')
      this.activeBody = menuItem
    }
  },
  components: {
    Navigation,
    Homepage,
    Footer,
    HelloWorld
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
}
</style>
