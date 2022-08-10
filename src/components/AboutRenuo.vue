<template>
  <div>
    <Team class="mt-5" />
    <Goodies class="mt-5" />
    <Checklist
      class="mt-5"
      title="Unser Angebot"
      :list="[
        'Eine top Ausbildung',
        'Spannende und vielseitige Projekte',
        'Neue Technologien',
        'Selbstständige Arbeitsweise',
        'Flexible Arbeitszeiten',
        'Ein technisch sehr kompetentes, kollegiales und junges Team',
        'Betreuung deine IPA',
        'Wir haben viele IMS-Abgänger unter uns und wissen genau, was auf dich zukommt!'
      ]"
    />
    <Tools class="mt-5" />
    <Location class="mt-5" />
    <IMSButton class="mt-5" />
  </div>
</template>

<script>
import Location from "@/components/Location";
import Team from "@/components/Team";
import Tools from "@/components/Tools";
import Goodies from "@/components/Goodies";

import "timeline-vuejs/dist/timeline-vuejs.css";
import IMSButton from "@/components/IMSButton";
import Checklist from "@/components/Checklist";

export default {
  name: "About Renuo",
  data() {
    return {
      hover: false
    };
  },
  components: {
    Checklist,
    IMSButton,
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
