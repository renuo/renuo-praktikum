<template>
  <div class="apply-now-container">
    <div class="h2">
      Wir sind bereit !
      <br />Du auch ?
      <br />
      <a href="https://www.renuo.ch/de/jobs/">
        Bewirb dich jetzt
      </a>
    </div>
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
    font-size: 2rem;
    color: white;
  }
  a:hover {
    border-bottom: 3px solid #fff;
  }
}
.h2 {
  color: #3a4440;
  font-size: 3rem;
  font-weight: bold;
}
</style>
