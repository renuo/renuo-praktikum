<template>
  <div>
    <h2>Standort</h2>
    <p class="subtitle">Hier findest du uns:</p>
    <div class="map img-fluid iframe-container" ref="iframeContainer">
      <iframe
        ref="iframe"
        style="height: 100%; width: 100%"
        class="img-fluid remove-border"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d219721.87235802517!2d8.508321660161725!3d47.35673387013604!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47900b1b31f3d935%3A0x4ac272717f6e976!2sRenuo%20AG!5e0!3m2!1sen!2sch!4v1597845570738!5m2!1sen!2sch"
        height="100%"
        width="80%"
        allowfullscreen=""
        aria-hidden="false"
        tabindex="0"
      ></iframe>
      <img class="cat" src="@/assets/about_renuo/cat.png" />
    </div>
    <blockquote class="text-center">
      "Aa zelle Bölle schelle, d’Chatz gaht uf Walliselle"
    </blockquote>
    <p class="text-center">
      🌟 2 Minuten vom <b>Bahnhof 🚂</b> entfernt<br />
      🌟 3 Minuten bis zur <b>Gastro-Oase 🍕</b><br />
      🌟 5 Minuten bis zum <b>Glattzentrum 🛍</b><br />
    </p>
  </div>
</template>

<script>
export default {
  name: "Location",
  methods: {
    replacemap: function() {
      console.log(this.$refs.iframe);
      let map = document.createElement("img");
      map.src = "~@/assets/map-fallback.png";
      this.$refs.iframeContainer.removeChild(this.$refs.iframe);
    }
  },
  mounted() {
    if (!window.navigator.onLine) {
      this.replacemap();
    }
    window.addEventListener("offline", () => this.replacemap());
  }
};
</script>

<style scoped lang="scss">
@use "@/stylesheets/global.scss";

.cat {
  width: 20vw;
  position: absolute;
  left: 0;
  bottom: 0;
  max-width: 150px;
}

.map {
  position: relative;
  background-image: url("~@/assets/map-fallback.png");
  background-size: contain;
  background-position: center;
  background-repeat: no-repeat;
}

.iframe-container {
  height: 60vh;
}

#locatin-listing {
  list-style-type: none;
  text-align: center !important;
}

blockquote {
  background: #f9f9f9;
  border-left: 10px solid #ccc;
  padding: 8px 10px;
}

p {
  text-align: center;
}
</style>
