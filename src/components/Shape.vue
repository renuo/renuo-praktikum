<template>
  <li ref="shape"></li>
</template>

<script>
export default {
  name: "Shape",
  mounted() {
    function createRandomShape(shape) {
      shape.style.left = `${Math.floor(Math.random() * 90)}%`;
      shape.style.width = `${Math.floor(Math.random() * 50) + 20}px`;
      shape.style.animationDuration = `${Math.floor(Math.random() * 30) + 40}s`;
    }

    createRandomShape(this.$refs.shape);
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
  bottom: calc(-150px - 40vh);
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
    transform: translateY(-3865px) rotate(360deg);
    opacity: 1;
  }
  100% {
    transform: translateY(-7730px) rotate(720deg);
    opacity: 0;
  }
}
</style>
