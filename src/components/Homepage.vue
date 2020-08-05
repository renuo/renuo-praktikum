<template>
  <div>
    <br />
    <span class="centered-text-banner"
      >Dein IMS Praktikum bei der Renuo AG</span
    >
    <br />
    <img
      alt="renuo-team"
      class="img-fluid image-block--centered"
      src="https://www.renuo.ch/images/renuo-landingpage-1a-dab40b370e94b1a9fbb951ee297870f9.jpg?vsn=d"
    />
  </div>
</template>
<script>
export default {
  name: "Navigation"
};
</script>

<style scoped lang="scss">
.img-fluid,
.video-fluid,
.blog-content img {
  max-width: 100%;
  height: auto;
  margin-top: 2%;
}
.centered-text-banner {
  font-size: 2rem !important;
  color: #27d79d;
  font-weight: bold;
}
@media (min-width: 1200px) {
  .img-fluid,
  .video-fluid,
  .blog-content img {
    max-width: 80%;
    height: auto;
    margin-top: 3%;
  }
}
</style>
