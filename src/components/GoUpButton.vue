<template>
  <a href="#navigationbar" id="go-up">
    <i class="fas fa-chevron-circle-up"></i>
  </a>
</template>

<script>
export default {
  name: "GoUp"
};

addEventListener("scroll", () => {
  if (window.scrollY === 0) {
    document.querySelector("a#go-up").style.display = null;
  } else {
    document.querySelector("a#go-up").style.display = "block";
  }
});
</script>

<style scoped lang="scss">
@use "@/stylesheets/variables.scss";
i {
  aspect-ratio: 1;
  font-size: 40px;
  color: variables.$renuo-base-color;
  background-color: #fff;
  border-radius: 50%;
  border: 2px solid #fff;
}

a {
  position: fixed;
  bottom: calc(5px + 4vw);
  right: calc(5px + 4vw);
  height: 44px;
  aspect-ratio: 1;
  display: none;
}
</style>
