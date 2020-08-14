<template>
  <div>
    <br />
    <span class="centered-text-banner"
      >Dein IMS Praktikum bei der Renuo AG</span
    >
    <br />
    <img alt="renuo team" class="img-fluid image-block--centered" :src="team" />

    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
    <br />
  </div>
</template>
<script>
import team from "@/assets/team.jpg";

export default {
  team: team,
  data() {
    return {
      team: team
    };
  }
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
