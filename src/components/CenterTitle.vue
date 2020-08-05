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
.title {
  font-weight: 500;
  color: #143327;
  text-align: center;
  font-size: 4rem;
  margin-top: 30px;
  line-height: 1.2;
}
@media (max-width: 991.98px) {
  .heading .title {
    font-size: 2.5rem;
    word-break: break-word;
    hyphens: auto;
  }
}
.background-header {
  background-color: #fff;
  min-height: 10rem;
  background-image: url(https://www.renuo.ch/images/header-6edb7e4d413dc5d722e34a8be66e8f06.svg?vsn=d);
  background-size: cover;
  background-repeat: no-repeat;
  background-position-y: bottom;
  z-index: -1;
}
</style>
