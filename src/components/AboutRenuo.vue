<template>
  <div>
    <Team />
    <Goodies />
    <Tools />
    <Location />
    <CustomerStatements />
  </div>
</template>

<script>
import Location from "@/components/Location";
import Team from "@/components/Team";
import Tools from "@/components/Tools";
import CustomerStatements from "@/components/CustomerStatements";
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
    CustomerStatements,
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
