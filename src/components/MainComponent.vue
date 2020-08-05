<template>
  <div>
    <Navigation @selected="setActive" />
    <CenterTitle id="about-renuo" title="Renuo" />
    <div class="content-container">
      <AboutRenuo />
    </div>
    <CenterTitle id="internship" title="Internship" />
    <Footer />
  </div>
</template>

<script>
import AboutRenuo from "./AboutRenuo.vue";
import CenterTitle from "./CenterTitle.vue";
import Footer from "./Footer.vue";
import Navigation from "./Navigation.vue";
import Vue from "vue";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
var VueScrollTo = require("vue-scrollto");
Vue.use(BootstrapVue);
Vue.use(IconsPlugin);
export default {
  name: "MainComponent",
  components: {
    AboutRenuo,
    CenterTitle,
    Footer,
    Navigation
  },
  methods: {
    isActive(menuItem) {
      return this.activeBody === menuItem;
    },
    setActive(menuItem) {
      this.activeBody = menuItem;
      VueScrollTo.scrollTo("#" + menuItem, 1500);
    }
  }
};
</script>
<style lang="scss">
.content-container {
  margin-left: auto;
  margin-right: auto;
  width: 80%;
}
</style>
