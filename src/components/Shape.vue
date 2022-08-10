<template>
  <li ref="shape"></li>
</template>

<script>
export default {
  name: "Shape",
  mounted() {
    this.createRandomShape(this.$refs.shape);
  },
  methods: {
    createRandomShape: function(shape) {
      shape.style.left = `${Math.floor(Math.random() * 90)}%`;
      shape.style.width = `${Math.floor(Math.random() * 50) + 20}px`;
      shape.style.animationDuration = `${Math.floor(Math.random() * 30) + 10}s`;
    }
  }
};
</script>

<style scoped lang="scss">
@use "@/stylesheets/variables.scss";

.circles li {
  position: absolute;
  display: block;
  list-style: none;
  background: variables.$renuo-base-color !important;
  animation: animate 60s linear infinite;
  bottom: 0;
  border-radius: 50%;
  border-top-left-radius: 0 !important;
  aspect-ratio: 1;
}

@keyframes animate {
  0% {
    transform: translateY(0) rotate(0deg);
    opacity: 0;
  }
  50% {
    transform: translateY(-50vh) rotate(360deg);
    opacity: 1;
  }
  100% {
    transform: translateY(-100vh) rotate(720deg);
    opacity: 0;
  }
}
</style>
