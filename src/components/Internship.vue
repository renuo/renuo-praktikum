<template>
  <div>
    <div>
      <div>
        <img class="centered-gallery-image" alt="Workspace" :src="work_space" />
      </div>
      <br />
      <br />
      <b-container>
        <b-row class="d-flex justify-content-center special_row">
          <b-col class="bubble-item col-12 col-md-12 col-lg-2 col-sm-12"
            ><div @click="showEinfuehrung">
              <Bubble
                centered
                text="Einfuehrung"
                title="August 2021"
                v-bind:radius="5"
              ></Bubble></div
          ></b-col>
          <b-col class="bubble-item col-12 col-md-12 col-lg-2 col-sm-12"
            ><div @click="showKundenprojekt">
              <Bubble
                centered
                text="Kundenprojekt"
                title="September 2021"
                v-bind:radius="5"
              ></Bubble></div
          ></b-col>
          <div class="bubble-item col-12 col-md-12 col-lg-2 col-sm-12">
            <div @click="showCoding">
              <Bubble
                centered
                title="Oktober 21 - August 22"
                text="Coding"
                v-bind:radius="7"
              ></Bubble>
            </div>
          </div>
          <b-col class="bubble-item col-12 col-md-12 col-lg-2 col-sm-12"
            ><div @click="showIPA">
              <Bubble
                centered
                text="IPA (5.0+)"
                title="September 2021"
                v-bind:radius="5"
              ></Bubble></div
          ></b-col>
          <b-col class="bubble-item col-12 col-md-12 col-lg-2 col-sm-12"
            ><div @click="showStudium">
              <Bubble
                centered
                text="Studium ?"
                title="September 2022"
                v-bind:radius="5"
              ></Bubble></div
          ></b-col>
        </b-row>
      </b-container>
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
                <i class="icon-li icon-ok"></i> Anforderungsanalyse, Technische
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
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import Vue from "vue";
import work_space from "@/assets/work_space.png";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";
Vue.use(BootstrapVue);
Vue.use(IconsPlugin);
import Bubble from "./Bubble.vue";
import VueSweetalert2 from "vue-sweetalert2";
// If you don't need the styles, do not connect
const options = {
  confirmButtonColor: "#27d79d",
  cancelButtonColor: "#27d79d"
};
import "sweetalert2/dist/sweetalert2.min.css";
Vue.use(VueSweetalert2, options);

export default {
  name: "Internship",
  components: {
    Bubble
  },
  data() {
    return {
      work_space: work_space
    };
  },
  methods: {
    showEinfuehrung() {
      this.$swal({
        title: "Einstieg",
        text:
          "Du wirst von den Mitarbeitern von Renuo in das Praktikum eingearbeitet und folgst einem detailierten Plan",
        icon: "info",
        showConfirmButton: false,
        showCloseButton: true,
        showClass: {
          popup: "animate__animated animate__fadeInDown"
        },
        hideClass: {
          popup: "animate__animated animate__fadeOutUp"
        }
      });
    },
    showKundenprojekt() {
      this.$swal({
        title: "Kundenproject",
        text:
          "Du arbeitest an einem eigenen Projekt und erzeugst Mehrwert für einen Kunden. Du wirst während dem Projekt vom Team unterstützt",
        icon: "info",
        showConfirmButton: false,
        showCloseButton: true,
        showClass: {
          popup: "animate__animated animate__fadeInDown"
        },
        hideClass: {
          popup: "animate__animated animate__fadeOutUp"
        }
      });
    },
    showCoding() {
      this.$swal({
        title: "Entwickeln !!",
        text:
          "Nun wird endlich Software entwickelt. Bleib dran und erfreue dich an der Hauptaufgabe deines Praktikums",
        icon: "info",
        showConfirmButton: false,
        showCloseButton: true,
        showClass: {
          popup: "animate__animated animate__fadeInDown"
        },
        hideClass: {
          popup: "animate__animated animate__fadeOutUp"
        }
      });
    },
    showIPA() {
      this.$swal({
        title: "IPA",
        text:
          "Der Abschluss der Schulischen Aufgaben. Bei Renuo unterstützten wir dich eine gute Note zu erreichen",
        icon: "info",
        showConfirmButton: false,
        showCloseButton: true,
        showClass: {
          popup: "animate__animated animate__fadeInDown"
        },
        hideClass: {
          popup: "animate__animated animate__fadeOutUp"
        }
      });
    },
    showStudium() {
      this.$swal({
        title: "Studieren",
        text:
          "Als Informatiker ist ein dauerhaftes Weiterbilden eine wichtige Komponente von Erfolg. Also ab ins Studium",
        icon: "info",
        showConfirmButton: false,
        showCloseButton: true,
        showClass: {
          popup: "animate__animated animate__fadeInDown"
        },
        hideClass: {
          popup: "animate__animated animate__fadeOutUp"
        }
      });
    }
  }
};
</script>
<style lang="scss" scoped>
.work_during_internship_section {
  padding-top: 25px;
  padding-bottom: 25px;
  text-align: center;
  font-size: 1rem;
}

.centered-gallery-image {
  width: 60%;
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
