<template>
  <div class="apply-now-container">
    <h2>
      Willst du dir einen besseren Einblick in unsere Projekte verschaffen?
    </h2>
    <a href="https://github.com/renuo/">GitHub</a>
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
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: variables.$renuo-base-color;
  a {
    margin-top: 20px;
    font-weight: normal;
    text-decoration: none;
    border-bottom: none;
    font-size: 1.5rem;
    color: white;
    padding-bottom: 1px;
  }
  a:hover {
    border-bottom: 1px solid #fff;
    padding-bottom: 0px;
  }
}
h2 {
  color: #3a4440;
  font-size: 2rem;
  font-weight: bold;
  padding-top: 20px;
  text-align: center;
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
