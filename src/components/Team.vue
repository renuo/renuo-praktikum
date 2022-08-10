<template>
  <div>
    <h2 id="about-renuo">Das Team</h2>
    <p class="subtitle">Weil wir mehr als nur Mitarbeiter sind</p>
    <a
      href="https://renuo.ch/team"
      class="btn btn-info"
      role="button"
      target="_blank"
      >Lerne das Team kennen</a
    >
    <img
      class="img-fluid"
      alt="renuo team"
      src="@/assets/about_renuo/team.png"
    />
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
@use "@/stylesheets/global.scss";

img {
  margin-top: -35px;
  pointer-events: none;
}

@media (min-width: 500px) {
  img {
    margin-top: -70px;
  }
}
</style>
