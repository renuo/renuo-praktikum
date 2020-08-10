<template>
  <div class="bouble_section">
    <div v-if="title">
      <span class="bouble-title">
        {{ title === "/" ? "-" : title }}
      </span>
    </div>
    <div :style="setColour" id="background_colour_div">
      <div :style="size" id="green-renuo-circle" v-bind:class="isCentered">
        <span class="inner-text">{{ text }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Bouble",
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
      required: true
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
  computed: {
    isCentered() {
      if (this.centered) {
        return "centered_bouble";
      } else {
        return "";
      }
    },
    size() {
      return {
        "--size": this.radius + "px"
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
.bouble-title {
  color: #27d79d;
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
  width: $size;
  height: $size;
  @extend .circle-text;
}
.centered_bouble {
  margin: 0 auto;
}
#green-renuo-circle {
  background-color: var(--background);
  color: white;
  font-weight: bold;
  @include circle-text(var(--size));
}
.bouble_section:hover {
  transform: scale(1.2);
}
</style>
