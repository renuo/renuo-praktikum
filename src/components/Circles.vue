<template>
  <div>
    <ul class="circles" ref="left-circles" style="left: 0"></ul>
    <ul class="circles" ref="right-circles" style="right: 0"></ul>
  </div>
</template>

<script>
import Shape from "@/components/Shape";
import Vue from "vue";

export default {
  name: "Circles",
  mounted() {
    if (window.innerWidth > 900) {
      this.addShape();
    }
  },
  methods: {
    addShape: function addShape() {
      const leftCircles = this.$refs["left-circles"];
      const rightCircles = this.$refs["right-circles"];
      const ComponentClass = Vue.extend(Shape);
      let instance = new ComponentClass();
      instance.$mount();
      leftCircles.appendChild(instance.$el);
      this.deleteShape(
        instance,
        parseInt(instance.$refs["shape"].style.animationDuration.slice(0, -1)) /
          0.001,
        leftCircles
      );
      instance = new ComponentClass();
      instance.$mount();
      rightCircles.appendChild(instance.$el);
      this.deleteShape(
        instance,
        parseInt(instance.$refs["shape"].style.animationDuration.slice(0, -1)) /
          0.001,
        rightCircles
      );
      if (window.innerWidth > 900) {
        setTimeout(
          () => this.addShape(),
          Math.floor(Math.random() * 4000 - window.innerWidth) + 200
        );
      }
    },
    deleteShape: function deleteShape(instance, delay, group) {
      setTimeout(() => {
        group.removeChild(instance.$el);
        instance.$destroy();
      }, delay);
    }
  }
};
</script>

<style scoped lang="scss">
.circles {
  position: fixed;
  top: 0;
  bottom: 0;
  height: 100vh;
  width: calc((100vw - 750px) / 2);
  z-index: 0;
  padding: 0;
}
</style>
