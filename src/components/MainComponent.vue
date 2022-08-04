<template>
  <div style="background: #ccd5db">
    <Navigation @selected="setActive" />
    <div style="padding: 0px 20px" class="main-content">
      <Internship />
      <AboutRenuo />
      <CenterTitle id="projects" title="Projekte" />
      <Projects />
      <Values />
      <Challenges />
      <Footer />
    </div>
  </div>
</template>
<script>
import Vue from "vue";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import AboutRenuo from "@/components/AboutRenuo";
import CenterTitle from "@/components/CenterTitle";
import Challenges from "@/components/Challenges";
import Footer from "@/components/Footer";
import Internship from "@/components/Internship";
import Navigation from "@/components/Navigation";
import Projects from "@/components/Projects";
import Values from "@/components/Values";

var VueScrollTo = require("vue-scrollto");
Vue.use(BootstrapVue);
Vue.use(IconsPlugin);
export default {
  name: "MainComponent",
  data: function() {
    return {
      inverted: false
    };
  },
  components: {
    AboutRenuo,
    CenterTitle,
    Challenges,
    Footer,
    Internship,
    Navigation,
    Projects,
    Values
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
@use "../stylesheets/variables.scss";

.main-content {
  max-width: 750px;
  margin: auto;
  background: variables.$default-background-color;
}
</style>
