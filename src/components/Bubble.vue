<template>
  <div class="bubble_section">
    <div v-if="title">
      <span class="bubble-title">
        {{ title === "/" ? "-" : title }}
      </span>
    </div>
    <div :style="setColour" id="background_colour_div">
      <div :style="size" id="green-renuo-circle" v-bind:class="isCentered">
        <fitty :options="options">
          <template v-slot:content>
            <span class="inner-text">{{ text }}</span>
          </template>
        </fitty>
      </div>
    </div>
  </div>
</template>

<script>
import Vue from "vue";

import Fitty from "vue-fitty";
Vue.use(Fitty);
export default {
  name: "Bubble",
  props: {
    radius: {
      type: Number,
      required: true
    },
    text: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: false
    },
    colour: {
      type: String,
      required: false
    },
    centered: {
      type: Boolean,
      required: false
    }
  },
  data: () => ({
    options: {
      minSize: 5,
      maxSize: 10
    }
  }),
  computed: {
    isCentered() {
      return this.centered ? "centered_bubble" : "";
    },
    size() {
      return {
        "--size": this.radius + "em"
      };
    },
    setColour() {
      return {
        "--background": this.colour ? this.colour : "#27d79d"
      };
    }
  }
};
</script>

<style lang="scss" scoped>
$default_font_size: var(--size);
$font_size: $default_font_size;

.bubble-title {
  color: #27d79d;
  white-space: pre-line;
  font-size: $font_size;
  overflow: hidden;
  white-space: nowrap;
}
.circle-text {
  position: relative;
  display: block;
  border-radius: 50%;
  text-align: center;
  .inner-text {
    display: block;
    @extend .center-align;
  }
}
.center-align {
  position: absolute;
  top: 50%;
  left: 50%;
  margin: auto;
  -webkit-transform: translateX(-50%) translateY(-50%);
  -ms-transform: translateX(-50%) translateY(-50%);
  transform: translateX(-50%) translateY(-50%);
}
@mixin circle-text($size) {
  width: var(--size);
  height: var(--size);
  @extend .circle-text;
}
.centered_bubble {
  margin: 0 auto;
}
#green-renuo-circle {
  background-color: var(--background);
  color: white;
  font-weight: bold;
  @include circle-text(var(--size));
}
.bubble_section:hover {
  transform: scale(1.2);
}
</style>
