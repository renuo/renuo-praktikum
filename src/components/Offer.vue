<template>
  <div>
    <h2>Unser Angebot</h2>
    <ul>
      <li><i class="fas fa-check"></i>Eine top Ausbildung</li>
      <li><i class="fas fa-check"></i>Spannende und vielseitige Projekte</li>
      <li><i class="fas fa-check"></i>Neue Technologien</li>
      <li><i class="fas fa-check"></i>Selbstständige Arbeitsweise</li>
      <li><i class="fas fa-check"></i>Flexible Arbeitszeiten</li>
      <li>
        <i class="fas fa-check"></i>Ein technisch sehr kompetentes, kollegiales
        und junges Team
      </li>
      <li><i class="fas fa-check"></i>Betreuung deine IPA</li>
      <li>
        <i class="fas fa-check"></i>Wir haben viele IMS-Abgänger unter uns und
        wissen genau, was auf dich zukommt!
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Offer"
};
</script>

<style scoped lang="scss">
@use "../stylesheets/global.scss";
@use "../stylesheets/variables.scss";
li {
  list-style-type: none;
  i {
    margin-right: 5px;
    color: variables.$renuo-base-color;
  }
}
</style>
