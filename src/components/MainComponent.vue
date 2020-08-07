<template>
  <div>
    <Navigation @selected="setActive" />
    <div class="content-container">
      <CenterTitle id="about-renuo" title="Renuo" />
      <AboutRenuo />
    </div>
    <div class="content-container">
      <CenterTitle id="internship" title="Internship" />
      <Homepage />
    </div>
    <Footer />
  </div>
</template>
<script>
import AboutRenuo from "./AboutRenuo.vue";
import CenterTitle from "./CenterTitle.vue";
import Footer from "./Footer.vue";
import Navigation from "./Navigation.vue";
import Homepage from "./Homepage.vue";
import Vue from "vue";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";

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
    Footer,
    Navigation,
    Homepage
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
