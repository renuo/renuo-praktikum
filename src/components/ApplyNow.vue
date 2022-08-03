<template>
  <div class="apply-now-container">
    <div class="h2"><br />Neugierig auf unsere Github-Projekte?</div>
  </div>
</template>

<script>
export default {
  name: "AboutRenuo"
};
</script>

<style scoped lang="scss">
@import "@/stylesheets/variables.scss";

.apply-now-container {
  margin-bottom: 50px;
  background-color: $renuo-base-color;
  a {
    font-weight: normal;
    transition: border-width 0.5s ease-in-out;
    text-decoration: none;
    border-bottom: 1px solid #fff;
    font-size: 1rem;
    color: white;
  }
  a:hover {
    border-bottom: 3px solid #fff;
  }
}
.h2 {
  color: #3a4440;
  font-size: 2rem;
  font-weight: bold;
}

@media (max-width: 500px) {
  .h2 {
    font-size: 2rem;
  }
  a {
    font-size: 1.6rem !important;
  }
  .apply-now-container {
    margin-bottom: -50px !important;
  }
}
</style>
