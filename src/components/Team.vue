<template>
  <div>
    <h2 id="about-renuo">Das Team</h2>
    <img class="img-fluid" alt="renuo team" src="@/assets/team.png" />
    <a href="https://renuo.ch/team" class="btn btn-info my-4" role="button"
      >Lerne das Team kennen</a
    >
  </div>
</template>
<script>
export default {
  name: "Team",
  data() {
    return {};
  }
};
</script>

<style scoped lang="scss">
@use "../stylesheets/global.scss";

img {
  margin-top: -35px;
}

@media (min-width: 500px) {
  img {
    margin-top: -70px;
  }
}
</style>
