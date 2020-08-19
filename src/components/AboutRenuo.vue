<template>
  <div class="my-container">
    <h3 class="h3-title" id="about-renuo">Dein künftiger Praktikumsort</h3>
    <br />
    <img class="img-full" alt="renuo team" :src="team" />
    <h3 class="h3-title">Tools</h3>
    <p>Damit arbeiten wir</p>
    <img class="img-padded" alt="tools" :src="tools" />
    <h3 class="h3-title">Standort</h3>
    <p>Hier findest du uns</p>
    <div class="map img-full iframe-container">
      <iframe
        class="img-full remove-border"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d219721.87235802517!2d8.508321660161725!3d47.35673387013604!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47900b1b31f3d935%3A0x4ac272717f6e976!2sRenuo%20AG!5e0!3m2!1sen!2sch!4v1597845570738!5m2!1sen!2sch"
        height="100%"
        width="80%"
        allowfullscreen=""
        aria-hidden="false"
        tabindex="0"
      ></iframe>
      <img class="cat" :src="cat" />
    </div>
    <blockquote>
      "Aa zelle Bölle schelle, d’Chatz gaht uf Walliselle"
    </blockquote>
    <div>
      <ul id="locatin-listing">
        <li>🌟 2 Minuten vom Bahnhof entfernt</li>
        <li>🌟 5 Minuten bis zum Glatzentrum</li>
      </ul>
    </div>
    <h3 class="h3-title">Kundenauszug</h3>
    <br />
    <img class="img-padded" alt="kundenauszug" :src="kundenauszug" />
    <br />
    <p>
      Die Stärke der Renuo zeigt sich in der Vielseitigkeit der Projekte, welche
      von den verschiedensten Branchen und Firmen beauftragt wurden.
    </p>
    <h3 class="h3-title">Fokus und Stärken</h3>
    <p>Wir entwickeln individuelle Software auf höchstem Niveau.</p>
    <ul class="values-listing">
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img class="values-img" alt="Quality and Precision" :src="w1" />
            </div>
            <div class="col-md-6 text-left text-col">
              <h2 class="values-title">Qualität und Präzision</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img
                class="values-img"
                alt="Fairness and Transparency"
                :src="w2"
              />
            </div>
            <div class="col-md-6 text-left text-col">
              <h2 class="values-title">Verantwortlichkeit</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img class="values-img" alt="Responsibility" :src="w3" />
            </div>
            <div class="col-md-6 text-left text-col">
              <h2 class="values-title">Gerechtigkeit und Transparenz</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img class="values-img" alt="Together" :src="w4" />
            </div>
            <div class="col-md-6 text-left text-col">
              <h2 class="values-title">Neue Wege</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img class="values-img" alt="New ways" :src="w5" />
            </div>
            <div class="col-md-6 text-left text-col">
              <h2 class="values-title">Zusammen</h2>
            </div>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
import cat from "@/assets/cat.png";
import w1 from "@/assets/w1.svg";
import w2 from "@/assets/w2.svg";
import w3 from "@/assets/w3.svg";
import w4 from "@/assets/w4.svg";
import w5 from "@/assets/w5.svg";
import team from "@/assets/team.jpg";
import tools from "@/assets/tools.png";
import kundenauszug from "@/assets/kundenauszug.png";

import "timeline-vuejs/dist/timeline-vuejs.css";

export default {
  name: "AboutRenuo",
  data() {
    return {
      cat: cat,
      w1: w1,
      w2: w2,
      w3: w3,
      w4: w4,
      w5: w5,
      team: team,
      tools: tools,
      kundenauszug: kundenauszug,
      hover: false
    };
  }
};
</script>

<style scoped lang="scss">
@import "@/stylesheets/custom_stylesheet.scss";

#locatin-listing {
  list-style-type: none;
  font-size: 1.75rem;
  text-align: center !important;
}

@media (max-width: 700px) {
  #locatin-listing {
    font-size: 1rem;
  }
}
</style>
