<template>
  <div>
    <CenterTitle id="projects" title="Projekte" />
    <div class="scroll-container">
      <div class="projects-container">
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
    </div>
    <CustomerStatements class="mt-5" />
  </div>
</template>

<script>
import CustomerStatements from "@/components/CustomerStatements";
import CenterTitle from "@/components/CenterTitle";

export default {
  name: "Projects",
  components: {
    CustomerStatements,
    CenterTitle
  },
  methods: {},
  data: function() {
    return {};
  }
};
</script>
<style scoped lang="scss">
.projects-container {
  width: 1500px;
  aspect-ratio: 700/260;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-between;
  align-items: center;
}

.scroll-container {
  overflow-x: scroll;
  overflow-y: hidden;
  white-space: nowrap;
  width: 100%;
  height: 100%;
}

div.projects-container a img {
  height: 100%;
}

div.projects-container a {
  height: 100%;
  transition: all 100ms ease-in-out;
}

div.projects-container a:hover {
  transform: scale(1.05);
}
</style>
