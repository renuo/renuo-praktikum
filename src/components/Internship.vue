<template>
  <div>
    <div>
      <div>
        <img class="centered-gallery-image" alt="Workspace" :src="work_space" />
      </div>
      <br />
      <br />
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
                in deier Freizeit
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
      </div>
    </div>
  </div>
</template>
<script>
import "timeline-vuejs/dist/timeline-vuejs.css";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
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
          "Du wirst von den Mitarbeitern von Renuo in das Praktikum eingearbeitet und folgst einem detailierten Plan"
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
        mainItemStyles: "background-color: #9bf542",
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
    work_space: work_space
  })
};
</script>
<style lang="scss" scoped>
.work_during_internship_section {
  padding-top: 25px;
  padding-bottom: 25px;
  text-align: center;
  font-size: 1rem;
}

.timeline-center {
  margin-left: auto;
  margin-right: auto;
}

.centered-gallery-image {
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

.bubble-item {
  margin-top: 10px;
}
.swal2-show {
  font-size: 2rem;
}

.apply-now {
  font-size: 1.5vw;
  background-color: #27d79d;
  margin-bottom: 5rem;
  padding: 1rem;
  background-image: url("http://renuo.ch/images/header-gray-c059a3ec41d8322d3e3fa1656b578ccb.svg?vsn=d");
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
