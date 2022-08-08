<template>
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
</template>

<script>
export default {
  name: "Projects",
  components: {},
  methods: {},
  data: function() {
    return {};
  }
};
</script>
<style scoped lang="scss">
div.projects-container {
  width: 100%;
  aspect-ratio: 700/260;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-between;
  align-items: center;
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
