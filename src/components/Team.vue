<template>
  <div>
    <CenterTitle id="about-renuo" title="Deine Firma" />
    <p class="subtitle">Weil wir mehr als nur Teammitglieder sind</p>
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
import CenterTitle from "@/components/CenterTitle";
export default {
  name: "Team",
  components: { CenterTitle },
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
