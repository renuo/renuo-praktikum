<template>
  <div>
    <h2>Fokus und Stärken</h2>
    <p class="text-center mx-4">
      Wir entwickeln für Kunden individuelle Software auf höchstem Niveau. Das
      sind unsere Werte:
    </p>
    <div class="values-container">
      <ul>
        <li><p>Qualität und Präzision</p></li>
        <li><p>Fairness und Transparenz</p></li>
        <li><p>Verantwortung</p></li>
        <li><p>Zusammen</p></li>
        <li><p>Neue Wege</p></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Values"
};
</script>

<style lang="scss">
@use "@/stylesheets/global.scss";
@use "@/stylesheets/variables.scss";

h4 {
  margin-bottom: 30px;
}

h2 {
  padding-bottom: 30px;
  padding-top: 30px;
}
div.values-container ul li:nth-child(1) {
  background-image: url("../assets/about_renuo/w1.svg");
}
div.values-container ul li:nth-child(2) {
  background-image: url("../assets/about_renuo/w2.svg");
}
div.values-container ul li:nth-child(3) {
  background-image: url("../assets/about_renuo/w3.svg");
}
div.values-container ul li:nth-child(4) {
  background-image: url("../assets/about_renuo/w4.svg");
}
div.values-container ul li:nth-child(5) {
  background-image: url("../assets/about_renuo/w5.svg");
}

div.values-container {
  padding-top: 30px;
}

@media screen and (max-width: 318px) {
  p {
    font-size: calc(0.5rem + 3vw) !important;
  }
}

.values-container {
  text-align: center;

  & > ul {
    display: inline-block;
    padding-left: 0;
    margin-left: 0;
  }

  li {
    background-repeat: no-repeat;
    background-size: contain;
    line-height: 30px;
    padding-left: 45px;
    list-style-type: none;
    &:not(:last-child) {
      margin-bottom: 20px;
    }
  }

  p {
    text-align: left;
    font-size: calc(1.275rem + 0.3vw);
  }
}
</style>
