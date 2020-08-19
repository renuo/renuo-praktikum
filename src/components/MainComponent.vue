<template>
  <div>
    <Navigation2 @selected="setActive" />
    <div class="content-container">
      <AboutRenuo />
    </div>
    <br /><br />

    <CenterTitle id="internship" title="Dein Praktikum bei uns" />
    <br />
    <Internship />
    <br />
    <div class="content-container">
      <CenterTitle id="projects" title="Projekte" />
      <br />
      <Projects />
    </div>
    <br /><br />
    <br />

    <div class="content-container">
      <CenterTitle id="challenges" title="Challenge" />
      <br />
      <Challenges />
    </div>
    <Footer />
  </div>
</template>
<script>
import * as TastyBurgerButton from "vue-tasty-burgers";
import Navigation2 from "./Navigation2.vue";
import AboutRenuo from "./AboutRenuo.vue";
import Footer from "./Footer.vue";
import CenterTitle from "./CenterTitle.vue";
import Projects from "./Projects.vue";
import Challenges from "./Challenges.vue";
import Internship from "./Internship.vue";
import Vue from "vue";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
var VueScrollTo = require("vue-scrollto");
Vue.use(BootstrapVue);
Vue.use(IconsPlugin);
Vue.use(TastyBurgerButton);
export default {
  name: "MainComponent",
  data: function() {
    return {
      inverted: false
    };
  },
  components: {
    Navigation2,
    AboutRenuo,
    CenterTitle,
    Internship,
    Projects,
    Challenges,
    Footer
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
body::-webkit-scrollbar {
  display: none;
}

body {
  -ms-overflow-style: none; /* IE and Edge */
  scrollbar-width: none; /* Firefox */
}

@mixin renuo-background {
  background-color: #27d79d !important;
  /*
		* Add font colour and other changes that are needed for green background
	*/
}

@mixin default-background {
  background-color: #fff;
  /*
		* Add font colour and other changes that are needed for green background
  */
}

$inverted: true !default;
.renuo_color_section {
  @include renuo-background;
}

.default_color_section {
  @include default-background;
}

.content-container {
  margin-left: auto;
  margin-right: auto;
}
</style>
