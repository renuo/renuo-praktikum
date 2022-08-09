<template>
  <div>
    <CenterTitle id="values" title="Fokus und Stärken" />
    <h4>Wir entwickeln individuelle Software auf höchstem Niveau.</h4>
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
    font-size: calc(1.325rem + 0.9vw);
  }
}
</style>
