<template>
  <div>
    <CenterTitle id="projects" title="Projekte" />
    <div class="scroll-container">
      <a href="https://mugshotbot.com/" target="_blank">
        <img src="@/assets/projects/msb.png" alt="mugshot bot" />
      </a>
      <a href="https://gifcoins.io/" target="_blank">
        <img src="@/assets/projects/gifcoins.png" alt="gifcoins" />
      </a>
      <a href="https://agreeder.com/" target="_blank">
        <img src="@/assets/projects/agreeder.png" alt="agreeder" />
      </a>
      <a href="https://www.auctionhub.io/" target="_blank">
        <img src="@/assets/projects/auctionhub.png" alt="auctionhub" />
      </a>
      <a href="https://www.citymessenger.ch/" target="_blank">
        <img src="@/assets/projects/citymessenger.png" alt="city messenger" />
      </a>
    </div>
    <CustomerStatements class="mt-5" />
    <Values class="mt-5" />
  </div>
</template>

<script>
import CustomerStatements from "@/components/CustomerStatements";
import CenterTitle from "@/components/CenterTitle";
import Values from "@/components/Values";

export default {
  name: "Projects",
  components: {
    CustomerStatements,
    CenterTitle,
    Values
  }
};
</script>
<style scoped lang="scss">
.scroll-container {
  overflow-x: scroll;
  overflow-y: hidden;
  white-space: nowrap;
  width: 100%;
  height: 100%;
  -webkit-overflow-scrolling: touch;
  scroll-behavior: smooth;
  scroll-snap-type: x mandatory;
  display: flex;
}

a {
  scroll-snap-align: start;
}
</style>
