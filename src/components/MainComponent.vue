<template>
  <div class="outer-container position-relative overflow-hidden">
    <Circles />
    <Navigation @selected="setActive" />
    <div class="main-content position-relative">
      <Internship />
      <Book />
      <AboutRenuo />
      <Projects style="margin-top: -80px" />
      <Challenges class="section-spacing" />

      <p class="text-center py-3">
        Made with<br />
        <span class="heart">❤️</span><br />
        by Renuo IMS Interns
        <CurrentYearComponent :increment="0" />
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
import GoUp from "@/components/GoUpButton";
import FooterMadeBy from "@/components/FooterMadeBy";
import Circles from "@/components/Circles";
import CurrentYearComponent from "@/components/CurrentYearComponent";
import Book from "@/components/Book";

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
    Circles,
    CurrentYearComponent,
    FooterMadeBy,
    GoUp,
    AboutRenuo,
    Challenges,
    Footer,
    Internship,
    Navigation,
    Projects,
    Book
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
  max-width: 900px;
  background: variables.$default-background-color;
  margin: 20px auto 80px;
  border-radius: 20px;
  box-shadow: 0 0 100px 0 rgb(0 0 0 / 10%);
}

.section-spacing {
  margin-top: 100px;
}
</style>
