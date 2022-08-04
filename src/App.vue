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
  text-align: center;
  color: #2c3e50;
  font-family: "Montserrat", sans-serif;
}

:root::-webkit-scrollbar {
  display: none;
}

* {
  box-sizing: border-box;
}
</style>
