<template>
  <div>
    <Team class="mt-5" />
    <Goodies class="mt-5" />
    <Tools class="mt-5" />
    <Location class="mt-5" />
  </div>
</template>

<script>
import Location from "@/components/Location";
import Team from "@/components/Team";
import Tools from "@/components/Tools";
import Goodies from "@/components/Goodies";

import "timeline-vuejs/dist/timeline-vuejs.css";

export default {
  name: "About Renuo",
  data() {
    return {
      hover: false
    };
  },
  components: {
    Location,
    Team,
    Tools,
    Goodies
  }
};
</script>

<style scoped lang="scss">
@use "../stylesheets/global.scss";
</style>
