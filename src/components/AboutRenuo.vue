<template>
  <div>
    <h2 class="h3-title" id="about-renuo">Das Team</h2>
    <img class="img-fluid" alt="renuo team" :src="team" />
    <h2 class="h3-title">Goodies</h2>
    <p>
      Komm zu uns, wir bieten dir nebst Coding-Erfahrung noch mehr Benefits.
      Lass Sie dir nicht entgehen.
    </p>
    <div>
      <a href="https://renuo.ch/jobs" class="btn btn-info" role="button"
        >Komm zu uns ins Team</a
      >
    </div>
    <img class="goodies-img-fluid" alt="goodies" :src="goodies" />
    <h2 class="h3-title">Tools</h2>
    <p>Mit diesen Werkzeugen arbeiten wir</p>
    <img class="img-fluid" alt="tools" :src="tools" />
    <Location />
    <h2 class="h3-title">Kundenauszug</h2>
    <img class="img-fluid" alt="kundenauszug" :src="kundenauszug" />
    <p>
      Die Stärke der Renuo zeigt sich in der Vielseitigkeit der Projekte, welche
      von den verschiedensten Branchen und Firmen beauftragt wurden.
    </p>
  </div>
</template>

<script>
import team from "@/assets/team.jpg";
import tools from "@/assets/tools.png";
import kundenauszug from "@/assets/kundenauszug.png";
import goodies from "@/assets/goodies.png";

import Location from "@/components/Location";

import "timeline-vuejs/dist/timeline-vuejs.css";

export default {
  name: "About Renuo",
  data() {
    return {
      team: team,
      tools: tools,
      kundenauszug: kundenauszug,
      goodies: goodies,
      hover: false
    };
  },
  components: {
    Location
  }
};
</script>

<style scoped lang="scss">
@use "../stylesheets/global.scss";


</>
