<template>
  <div id="app">
    <MainComponent />
  </div>
</template>
<script>
import MainComponent from "@/components/MainComponent";
export default {
  name: "App",
  data() {
    return {
      activeBody: "home"
    };
  },

  components: {
    MainComponent
  }
};
</script>
<style lang="scss">
#app {
  color: #2c3e50;
  font-family: "Montserrat", sans-serif;
}

* {
  box-sizing: border-box;
}
</style>
