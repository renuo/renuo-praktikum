<template>
  <footer>
    <div class="curved-footer">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path
          fill="#27d79d"
          fill-opacity="1"
          d="M0,96L48,112C96,128,192,160,288,160C384,160,480,128,576,101.3C672,75,768,53,864,37.3C960,21,1056,11,1152,26.7C1248,43,1344,85,1392,106.7L1440,128L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"
        ></path>
      </svg>
    </div>
    <div class="footer-content"></div>
  </footer>
</template>
<script>
export default {
  name: "Footer"
};
</script>
<style scoped lang="scss">
footer {
  margin-top: auto;
  bottom: 0;
  width: 100%;
  height: 2.5rem;

  .footer-content {
    background-color: #27d79d;
  }
}
</style>
