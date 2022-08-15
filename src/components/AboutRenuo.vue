<template>
  <div>
    <Team class="mt-5" />
    <Goodies class="mt-5" />
    <Values class="mt-5" />
    <Tools class="mt-5" />
    <Location class="mt-5" />

    <IMSButton class="mt-5" id="ims" />
  </div>
</template>

<script>
import Location from "@/components/Location";
import Team from "@/components/Team";
import Tools from "@/components/Tools";
import Goodies from "@/components/Goodies";

import "timeline-vuejs/dist/timeline-vuejs.css";
import IMSButton from "@/components/IMSButton";
import Values from "@/components/Values";

export default {
  name: "About Renuo",
  data() {
    return {
      hover: false
    };
  },
  components: {
    Values,
    IMSButton,
    Location,
    Team,
    Tools,
    Goodies
  }
};
</script>

<style scoped lang="scss">
@use "@/stylesheets/global.scss";
</style>
