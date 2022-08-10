<template>
  <div>
    <h2>Unsere Werte</h2>
    <p class="text-center mx-4">
      Wir entwickeln individuelle Software auf höchstem Niveau. Dies sind unsere
      Werte:
    </p>
    <div class="values-container">
      <ul>
        <li><p>Qualität und Präzision</p></li>
        <li><p>Fairness und Transparenz</p></li>
        <li><p>Verwantwortung</p></li>
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

div.values-container ul li:nth-child(1) {
  background-image: url("../assets/w1.svg");
}
div.values-container ul li:nth-child(2) {
  background-image: url("../assets/w2.svg");
}
div.values-container ul li:nth-child(3) {
  background-image: url("../assets/w3.svg");
}
div.values-container ul li:nth-child(4) {
  background-image: url("../assets/w4.svg");
}
div.values-container ul li:nth-child(5) {
  background-image: url("../assets/w5.svg");
}

.values-container {
  text-align: center;

  & > ul {
    display: inline-block;
    margin-left: 35px;
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
