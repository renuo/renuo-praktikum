<template>
  <div>
    <h2 class="h3-title">Kundenauszug</h2>
    <p>
      Die Stärke der Renuo zeigt sich in der Vielseitigkeit der Projekte, welche
      von den verschiedensten Branchen und Firmen beauftragt wurden.
    </p>
    <img class="img-fluid" alt="kundenauszug" src="@/assets/kundenauszug.png" />
    <div class="customer-container">
      <img
        src="@/assets/customer_statements/jumbo.png"
        alt="jumbo-icon"
        id="jumbo"
      />
      <!-- <img src="@/assets/customer_statements/.png" /> -->
    </div>
  </div>
</template>

<script>
export default {
  name: "Customer_statements"
};
</script>

<style scoped lang="scss">
@use "../stylesheets/global.scss";
div.customer-container {
  aspect-ratio: 720/405;
  width: 100%;
  border: 1px black solid;
  position: relative;
}

div.customer-container > * {
  position: absolute;
  display: block;
}

img#jumbo {
  aspect-ratio: 57/23;
  height: 5.7%;
  left: 7.8%;
  top: 40.5%;
}
</style>
