<template>
  <div class="apply-now-container">
    <div class="h2">
      WIllst du dir einen besseren Einblick in unsere Projekte verschaffen?
    </div>
    <a href="https://github.com/renuo/">Github</a>
  </div>
</template>

<script>
export default {
  name: "AboutRenuo"
};
</script>

<style scoped lang="scss">
@use "../stylesheets/variables.scss";

.apply-now-container {
  margin-bottom: 50px;

  background-color: variables.$renuo-base-color;
  a {
    margin-top: 20px;
    font-weight: normal;
    text-decoration: none;
    border-bottom: none;
    font-size: 1.5rem;
    color: white;
  }
  a:hover {
    border-bottom: 1px solid #fff;
  }
}
.h2 {
  color: #3a4440;
  font-size: 2rem;
  font-weight: bold;
  padding-top: 20px;
}

@media (max-width: 500px) {
  .h2 {
    font-size: 2rem;
  }
  .apply-now-container {
    margin-bottom: -50px !important;
  }
}
</style>
