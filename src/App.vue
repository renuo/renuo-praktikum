<template>
<div id="app">
<Navigation @selected="setActive"/>
<CenterTitle id="about-renuo" title="Renuo"></CenterTitle>
<div class="content-container"><AboutRenuo></AboutRenuo></div>
<CenterTitle id="internship" title="Internship"></CenterTitle>
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
import CenterTitle from './components/CenterTitle.vue'
import Vue from 'vue'
var VueScrollTo = require('vue-scrollto')
// Install BootstrapVue
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)
export default {
  name: 'App',
  data () {
    return {
      activeBody: 'home'
    }
  },
  methods: {
    isActive (menuItem) {
      return this.activeBody === menuItem
    },
    setActive (menuItem) {
      this.activeBody = menuItem
      VueScrollTo.scrollTo('#' + menuItem, 1500)
    }
  },
  components: {
    Navigation,
    AboutRenuo,
    Footer,
    CenterTitle
  }
}
</script>
<style lang="scss">
  #app {
    font-family: Montserrat, Helvetica, Arial, sans-serif;
    text-align: center;
    color: #2c3e50;
    font-family: 'Montserrat', sans-serif;
  }
  .content-container{
    margin-left: auto;
    margin-right:auto;
    width:80%;
  }
</style>
