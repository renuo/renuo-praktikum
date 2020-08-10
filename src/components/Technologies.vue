<template>
  <div>
    <div :id="getSliderID('')" class="carousel slide" data-ride="carousel">
      <ol class="carousel-indicators">
        <li v-for="(tech, index) in this.technologies" :key="tech.technology">
          <div
            :data-target="getSliderID('#')"
            :data-slide-to="index"
            class="active"
          ></div>
        </li>
      </ol>
      <div class="carousel-inner">
        <div v-for="(tech, index) in this.technologies" :key="tech.technology">
          <Technology
            :image="tech.image"
            :technology="tech.technology"
            :active="index == 0"
          />
        </div>
      </div>
      <a
        class="carousel-control-prev"
        :href="getSliderID('#')"
        role="button"
        data-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a
        class="carousel-control-next"
        :href="getSliderID('#')"
        role="button"
        data-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>
  </div>
</template>

<script>
import Technology from "./Technology.vue";
export default {
  name: "Technologies",
  components: {
    Technology
  },
  props: {
    technologies: {
      type: Array,
      required: false
    },
    name: {
      type: String,
      required: false
    }
  },
  methods: {
    getSliderID(prefix) {
      var id = prefix + this.slugify(this.name.toLowerCase());
      return id;
    },
    slugify(str) {
      str = str.replace(/^\s+|\s+$/g, "");

      // Make the string lowercase
      str = str.toLowerCase();

      // Remove accents, swap ñ for n, etc
      var from =
        "ÁÄÂÀÃÅČÇĆĎÉĚËÈÊẼĔȆÍÌÎÏŇÑÓÖÒÔÕØŘŔŠŤÚŮÜÙÛÝŸŽáäâàãåčçćďéěëèêẽĕȇíìîïňñóöòôõøðřŕšťúůüùûýÿžþÞĐđßÆa·/_,:;";
      var to =
        "AAAAAACCCDEEEEEEEEIIIINNOOOOOORRSTUUUUUYYZaaaaaacccdeeeeeeeeiiiinnooooooorrstuuuuuyyzbBDdBAa------";
      for (var i = 0, l = from.length; i < l; i++) {
        str = str.replace(new RegExp(from.charAt(i), "g"), to.charAt(i));
      }

      // Remove invalid chars
      str = str
        .replace(/[^a-z0-9 -]/g, "")
        // Collapse whitespace and replace by -
        .replace(/\s+/g, "-")
        // Collapse dashes
        .replace(/-+/g, "-");

      return str;
    }
  }
};
</script>
<style scoped lang="scss"></style>
