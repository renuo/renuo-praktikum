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

<style scoped>
i {
  position: fixed;
  bottom: 20px;
  right: 20px;
  aspect-ratio: 1;
  font-size: 40px;
  color: #27d79d;
  background-color: #fff;
  border-radius: 50%;
  border: 2px solid #fff;
}

a {
  height: 75px;
  aspect-ratio: 1;
  display: none;
}
</style>
