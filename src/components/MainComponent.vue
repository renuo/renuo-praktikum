<template>
  <div class="outer-container">
    <Navigation @selected="setActive" />
    <div class="main-content">
      <Internship />
      <AboutRenuo />

      <Projects class="section-spacing" />
      <Values class="mt-5" />

      <Challenges class="section-spacing" />

      <p class="text-center py-3">
        Made with<br />
        <span class="heart">❤️</span><br />
        by Renuo IMS Interns <CurrentYearComponent :increment="0" />
      </p>
    </div>
    <Footer />
    <FooterMadeBy />
    <GoUp />
  </div>
</template>
<script>
import Vue from "vue";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import AboutRenuo from "@/components/AboutRenuo";
import Challenges from "@/components/Challenges";
import Footer from "@/components/Footer";
import Internship from "@/components/Internship";
import Navigation from "@/components/Navigation";
import Projects from "@/components/Projects";
import Values from "@/components/Values";
import GoUp from "@/components/GoUpButton";
import FooterMadeBy from "@/components/FooterMadeBy";
import CurrentYearComponent from "@/components/CurrentYearComponent";

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
    CurrentYearComponent,
    FooterMadeBy,
    GoUp,
    AboutRenuo,
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
@use "@/stylesheets/variables.scss";

.main-content {
  max-width: 770px;
  background: variables.$default-background-color;
  margin: 20px auto auto;
  border-radius: 10px;
}

.outer-container {
  background: #f3f5f7;
}

.section-spacing {
  margin-top: 100px;
}
</style>
