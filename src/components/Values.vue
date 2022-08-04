<template>
  <div>
    <CenterTitle id="values" title="Fokus und Stärken" />
    <p>Wir entwickeln individuelle Software auf höchstem Niveau.</p>

    <div class="row">
      <div class="col-4 text-right">
        <img alt="Qualität und Präzision" src="@/assets/w1.svg" />
      </div>
      <div class="col-8 text-left">
        <h2>
          Qualität und<br />
          Präzision
        </h2>
      </div>
      <div class="w-100 mb-3"></div>
      <div class="col-4 text-right">
        <img alt="Fairness und Transparenz" src="@/assets/w2.svg" />
      </div>
      <div class="col-8 text-left">
        <h2>
          Fairness und<br />
          Transparenz
        </h2>
      </div>
      <div class="w-100 mb-3"></div>
      <div class="col-4 text-right">
        <img alt="Verantwortung" src="@/assets/w3.svg" />
      </div>
      <div class="col-8 text-left">
        <h2>Verantwortung</h2>
      </div>
      <div class="w-100 mb-3"></div>
      <div class="col-4 text-right">
        <img alt="Zusammen" src="@/assets/w4.svg" />
      </div>
      <div class="col-8 text-left">
        <h2>Zusammen</h2>
      </div>
      <div class="w-100 mb-3"></div>
      <div class="col-4 text-right">
        <img alt="Neue Wege" src="@/assets/w5.svg" />
      </div>
      <div class="col-8 text-left">
        <h2>Neue Wege</h2>
      </div>
    </div>
  </div>
</template>

<script>
import CenterTitle from "@/components/CenterTitle";

export default {
  name: "Values",
  components: {
    CenterTitle
  }
};
</script>

<style lang="scss"></style>
