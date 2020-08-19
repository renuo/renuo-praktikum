<template>
  <div class="background-header">
    <div class="heading">
      <h1 class="title">
        {{ title }}
      </h1>
    </div>
  </div>
</template>

<script>
export default {
  name: "CenterTitle",
  props: {
    title: {
      type: String,
      required: true
    }
  }
};
</script>
<style scoped lang="scss">
@import "@/stylesheets/variables.scss";

.title {
  width: 100% !important;
  color: $renuo-base-color;
  font-size: 5rem;
  font-weight: 500;
  padding-top: 8rem;
  margin: auto;
  padding-bottom: 5rem;
  margin-top: -5rem;
}

.background-header {
  margin-top: 80px;
  background-color: #fff;
  background-image: url(https://www.renuo.ch/images/header-6edb7e4d413dc5d722e34a8be66e8f06.svg?vsn=d);
  background-size: cover;
  background-repeat: no-repeat;
  background-position-y: bottom;
  z-index: -1;
}

@media (max-width: 1200px) {
  .title {
    font-size: 4rem;
    padding-top: 3rem;
    padding-bottom: 3rem;
  }
  .background-header {
    margin-top: 60px;
  }
}

@media (max-width: 1000px) {
  .title {
    font-size: 3.5rem;
    padding-top: 3rem;
    padding-bottom: 3rem;
  }
}

@media (max-width: 500px) {
  .title {
    font-size: 2.5rem;
    padding: 25px;
  }
  .background-header {
    margin-top: 25px;
  }
}
</style>
