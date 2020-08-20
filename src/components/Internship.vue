<template>
  <div>
    <div>
      <div>
        <img class="centered-gallery-image" alt="Workspace" :src="work_space" />
      </div>
      <br />
      <br />
      <div id="dummy-line-item-for-image-insertion">
        <section
          data-v-7f3aebf1=""
          data-v-6f737b7e=""
          class="timeline timeline-center"
        >
          <div data-v-7f3aebf1="" class="wrapper-timeline">
            <div data-v-7f3aebf1="" class="wrapper-item">
              <div data-v-7f3aebf1="" class="section-year">
                <p data-v-7f3aebf1="" class="year"></p>
              </div>
              <section data-v-7f3aebf1="" class="timeline-item">
                <div data-v-818295b8="" id="" class="item">
                  <h3 data-v-818295b8="" class="date-item"></h3>
                  <h4 data-v-818295b8="" class="title-item"></h4>
                  <p data-v-818295b8="" class="description-item"></p>
                </div>
              </section>
            </div>
          </div>
        </section>
      </div>
      <div>
        <section
          data-v-7f3aebf1=""
          data-v-6f737b7e=""
          class="timeline timeline-center"
        >
          <div data-v-7f3aebf1="" class="wrapper-timeline">
            <div data-v-7f3aebf1="" class="wrapper-item">
              <div data-v-7f3aebf1="" class="section-year">
                <p data-v-7f3aebf1="" class="year"></p>
              </div>
              <section data-v-7f3aebf1="" class="timeline-item">
                <div data-v-818295b8="" id="" class="item">
                  <h3 data-v-818295b8="" class="date-item"></h3>
                  <h4 data-v-818295b8="" class="title-item"></h4>
                  <p data-v-818295b8="" class="description-item"></p>
                </div>
              </section>
            </div>
          </div>
        </section>
      </div>
      <Timeline
        class="timeline-center"
        :timeline-items="timelineItems"
        :colorDots="colorDots"
        :dateLocale="dateLocale"
        :shortToYearFormat="shortToYearFormat"
        :message-when-no-items="messageWhenNoItems"
      />
      <div class="work_during_internship_section center-layout">
        Während deines Praktikums wirst du dich mit vielen verschiedenen
        Technologien auseinandersetzten - unter anderem mit Ruby on Rails,
        Angular und React. Du wirst für Kunden einen Mehrwert generieren und
        durch die praktische Arbeit viel Erfahrung sammeln, ganz im Sinne von
        Learning by Doing. Unsere Praktikant*innen beteiligen sich weiter auch
        an Pair Programming, wodurch sie schnell Einblick in unsere Projekte
        erhalten und sich an unsere Methoden und Techniken gewöhnen.
      </div>
    </div>
    <h2 class="h3-title">Fokus und Stärken</h2>
    <p>Wir entwickeln individuelle Software auf höchstem Niveau.</p>
    <ul class="values_listing">
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
    <div class="pl-md-5 job-container">
      <div class="row mt-5 job-desc justify-content-between">
        <div class="col-12 col-md-12 col-lg-4 col-sm-12">
          <h3>Deine Mission</h3>
          <ul class="ul--jobs ul--jobs-detail">
            <ul class="icons-ul">
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Softwareentwicklung mit
                Webtechnologien (Ruby on Rails / Angular / HTML5 / Javascript)
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Anforderungsanalyse, technische
                Betreuung und Beratung von Kunden
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Datenbankdesign mit SQL (MySQL,
                Postgres)
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Mitwirkung im Projektmanagement
                mit <a href="/de/scrum">Scrum</a>
              </li>
              <br />
            </ul>
          </ul>
        </div>
        <div class="col-12 col-md-12 col-lg-4 col-sm-12">
          <h3>Was erwarten wir?</h3>
          <ul class="ul--jobs ul--jobs-detail">
            <ul class="icons-ul">
              <br />
              <li><i class="icon-li icon-ok"></i> Du ♥️ Open Source</li>
              <br />
              <li><i class="icon-li icon-ok"></i> Du hast gute Noten</li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Du programmierst manchmal auch
                in deiner Freizeit
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Du lernst gerne neue Dinge
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Du willst mit Linux oder Mac
                arbeiten
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Du kannst sehr selbständig
                arbeiten
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Du kannst klar kommunizieren
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Ein Plus: Du kennst Ruby oder
                Ruby on Rails, Javascript, TypeScript oder Coffeescript,
                AngularJS, SSH, Linux-Server oder andere Webtechnologien (z.B.
                Python, Django, PHP, JSF)
              </li>
              <br />
            </ul>
          </ul>
        </div>
        <div class="col-12 col-md-12 col-lg-4 col-sm-12">
          <h3>Was bieten wir?</h3>
          <ul class="ul--jobs ul--jobs-detail">
            <ul class="icons-ul">
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Spannende und vielseitige
                Projekte
              </li>
              <br />
              <li><i class="icon-li icon-ok"></i> Neue Technologien</li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Selbsständige Arbeitsweise
              </li>
              <br />
              <li><i class="icon-li icon-ok"></i> Flexible Arbeitszeiten</li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Ein technisch sehr kompetentes,
                motiviertes, kollegiales und junges Team
              </li>
              <br />
              <li><i class="icon-li icon-ok"></i> Betreuung deiner IPA</li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Wir haben viele IMS-Abgänger
                unter uns und wissen genau, was auf dich zukommt!
              </li>
              <br />
            </ul>
          </ul>
        </div>
        <div
          id="center-goodies-row"
          class="col-12 col-md-12 col-lg-12 col-sm-12"
        >
          <h3>Noch mehr Goodies</h3>
          <ul class="ul--jobs ul--jobs-detail center-goodies-row">
            <ul class="icons-ul">
              <br />
              <li>
                <i class="icon-li icon-ok"></i> Einmal jährliche Learning Week
                (2015 nach Sizilien, 2016 nach Lissabon, 2017 an den Comer See,
                2018 & 2019 im Elsass)
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i>½ Tag pro Woche für die
                eigenverantwortliche Weiterbildung
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i>Regelmässige Meetups und
                Konferenzbesuche
              </li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i>Kaffee (wir haben eine Bialetti
                :-)) und echten, chinesischen Tee
              </li>
              <br />
              <li><i class="icon-li icon-ok"></i> Früchte und Snacks</li>
              <br />
              <li>
                <i class="icon-li icon-ok"></i>Regelmässige Events (Team
                Ausflüge, Monthly Beers, Skitag, Weihnachtsessen)
              </li>
              <br />
            </ul>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import "timeline-vuejs/dist/timeline-vuejs.css";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import w1 from "@/assets/w1.svg";
import w2 from "@/assets/w2.svg";
import w3 from "@/assets/w3.svg";
import w4 from "@/assets/w4.svg";
import w5 from "@/assets/w5.svg";
import Vue from "vue";
import work_space from "@/assets/work_space.png";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";
Vue.use(BootstrapVue);
Vue.use(IconsPlugin);
// If you don't need the styles, do not connect
import Timeline from "./Timeline.vue";

var current_year = new Date().getFullYear();
export default {
  name: "Internship",
  components: {
    Timeline
  },
  data: () => ({
    dateLocale: "de-DE",
    colorDots: "#27d79d",
    shortToYearFormat: false,
    timelineItems: [
      {
        from: new Date(current_year + 1, 7),
        title: "Einführung",
        description:
          "Du wirst von den Mitarbeitern von Renuo in das Praktikum eingearbeitet und folgst einem detailierten <a href='assets/praktikumskonzept_2020.pdf' style='color: #27d79d' download>Plan</a>"
      },
      {
        from: new Date(current_year + 1, 8),
        title: "Kundenprojekt",
        description:
          "Du arbeitest an einem eigenen Projekt und erzeugst Mehrwert für einen Kunden. Du wirst während dem Projekt vom Team unterstützt"
      },
      {
        from: new Date(current_year + 1, 9),
        to: new Date(current_year + 2, 2),
        isMainTimeEntry: true,
        mainItemStyles: "background-color: #28d79d7d",
        title: "Coden",
        description:
          "Nun wird endlich Software entwickelt. Bleib dran und erfreue dich an der Hauptaufgabe deines Praktikums"
      },
      {
        from: new Date(current_year + 2, 2),
        title: "IPA (5+)",
        description:
          "Der Abschluss der Schulischen Aufgaben. Bei Renuo unterstützten wir dich eine gute Note zu erreichen"
      },
      {
        from: new Date(current_year + 2, 8),
        title: "Studium (Arbeiten)",
        description:
          "Nach deinem Praktikum hast du die Möglichkeit ein Studium zu beginnen oder weiter bei uns zu arbeiten"
      }
    ],
    work_space: work_space,
    w1: w1,
    w2: w2,
    w3: w3,
    w4: w4,
    w5: w5
  })
};
</script>
<style lang="scss" scoped>
@import "@/stylesheets/custom_stylesheet.scss";

.work_during_internship_section {
  padding-top: 25px;
  padding-bottom: 25px;
  text-align: center;
  font-size: 1rem;
}

@media (max-width: 700px) {
  .work_during_internship_section {
    text-align: left !important;
    width: 90% !important;
  }
  .centered-gallery-image {
    width: 75% !important;
  }
}

.timeline-center {
  margin-left: auto;
  margin-right: auto;
}

.values_listing {
  list-style-type: none;
}

.centered-gallery-image {
  z-index: 1;
  position: relative;
  width: 60%;
  border-radius: 10px;
  height: auto;
  margin: auto;
}

.job-desc {
  margin-bottom: 0.5rem;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  margin-bottom: 0.5rem !important;
  font-weight: 500 !important;
  line-height: 1.2 !important;
}

.center-layout {
  width: 60%;
  margin: auto;
}
.job-container {
  max-width: 80% !important;
  width: 80% !important;
  margin: auto;
  h3 {
    font-weight: bold !important;
  }
}

#dummy-line-item-for-image-insertion {
  z-index: -1;
  margin-top: -120px;
}

.ul--jobs-detail {
  list-style-image: url(https://www.renuo.ch/images/check-ddee0b6009fa00fff3365f0a93ccefb3.png?vsn=d);
  li {
    display: list-item;
    text-align: left !important;
    line-height: 2rem;
    a {
      font-weight: 200;
      padding-bottom: 0.25rem;
      border-bottom: 1px solid #27d79d;
      color: #27d79d;
      transition: all 0.5s;
    }
  }
}

.swal2-show {
  font-size: 2rem;
}

.apply-now {
  font-size: 1.5vw;
  background-color: #27d79d;
  margin-bottom: 5rem;
  padding: 1rem;
  background-image: url("https://renuo.ch/images/header-gray-c059a3ec41d8322d3e3fa1656b578ccb.svg?vsn=d");
}

@media (max-width: 1200px) {
  .apply-now {
    font-size: 2.5vw;
  }
}

@media (max-width: 1207px) {
  .ul--jobs-detail {
    padding-inline-start: 0px !important;
  }
}

@media (max-width: 750px) {
  .ul--jobs-detail {
    padding-inline-start: 5px !important;
  }
}

@media (max-width: 500px) {
  .apply-now {
    font-size: 4.5vw;
  }
}
@media (max-width: 500px) {
  .apply-now {
    font-size: 4.5vw;
  }
  .ul--jobs-detail {
    ul {
      font-size: 0.8rem;
      padding-inline-start: 5px !important;
    }
  }
}
@media (max-width: 450px) {
}
</style>
