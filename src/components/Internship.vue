<template>
  <div class="center-layout">
    <div>
      <img
        class="centered-gallery-image"
        alt="Fairness and Transparency"
        :src="internship_book"
      />
    </div>
    <br />
    <b-container>
      <b-row>
        <b-col
          ><div @click="showEinfuehrung">
            <Bubble
              centered
              text="Einfuehrung"
              title="August 21"
              v-bind:radius="5"
            ></Bubble></div
        ></b-col>
        <b-col
          ><div @click="showKundenprojekt">
            <Bubble
              centered
              text="Kundenprojekt"
              title="September 21"
              v-bind:radius="5"
            ></Bubble></div
        ></b-col>
        <b-col
          ><div @click="showCoding">
            <Bubble
              centered
              title="August - September"
              text="Coding"
              v-bind:radius="8"
            ></Bubble></div
        ></b-col>
        <b-col
          ><div @click="showIPA">
            <Bubble
              centered
              text="IPA (5.0+)"
              title="September 21"
              v-bind:radius="5"
            ></Bubble></div
        ></b-col>
        <b-col
          ><div @click="showStudium">
            <Bubble
              centered
              text="Studium"
              title="September 22"
              v-bind:radius="5"
            ></Bubble></div
        ></b-col>
      </b-row>
    </b-container>
    <div class="work_during_internship_section">
      Waehrend deines Praktikums wirst du dich vielen verschiedenen Technologien
      konfrontiert sehen. Darunter sind Ruby on Rails, Angular, React und andere
      Web Technologien. Du wirst fuer Kunden einen Mehrwert generieren und
      groesstenteils durch das Arbeiten an Erfahrung gewinnen. Also learning by
      doing. Es ist ebenfalls ein Wunsch vom Team dass sich die Praktikanten an
      Pair Programming beteiligen und dadurch schneller in die Projekte
      eingearbeite bist und dich an die Methodik und Techniken der Renuo
      gewoehnst und anpasst.
    </div>
    <div class="row mt-5 job-desc justify-content-between">
      <div class="col-12 col-md-6 col-lg-4 mt-4">
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
      <div class="col-12 col-md-6 col-lg-4 mt-4">
        <h3>Was erwarten wir?</h3>
        <ul class="ul--jobs ul--jobs-detail">
          <ul class="icons-ul">
            <br />
            <li><i class="icon-li icon-ok"></i> Du ♥️ Open Source</li>
            <br />
            <li><i class="icon-li icon-ok"></i> Du hast gute Noten</li>
            <br />
            <li>
              <i class="icon-li icon-ok"></i> Du programmierst manchmal auch in
              deier Freizeit
            </li>
            <br />
            <li><i class="icon-li icon-ok"></i> Du lernst gerne neue Dinge</li>
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
              <i class="icon-li icon-ok"></i> Ein Plus: Du kennst Ruby oder Ruby
              on Rails, Javascript, TypeScript oder Coffeescript, AngularJS,
              SSH, Linux-Server oder andere Webtechnologien (z.B. Python,
              Django, PHP, JSF)
            </li>
            <br />
          </ul>
        </ul>
      </div>
      <div class="col-12 col-md-6 col-lg-4 mt-4">
        <h3>Was bieten wir?</h3>
        <ul class="ul--jobs ul--jobs-detail">
          <ul class="icons-ul">
            <br />
            <li>
              <i class="icon-li icon-ok"></i> Spannende und vielseitige Projekte
            </li>
            <br />
            <li><i class="icon-li icon-ok"></i> Neue Technologien</li>
            <br />
            <li><i class="icon-li icon-ok"></i> Selbsständige Arbeitsweise</li>
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
              <i class="icon-li icon-ok"></i> Wir haben viele IMS-Abgänger unter
              uns und wissen genau, was auf dich zukommt!
            </li>
            <br />
          </ul>
        </ul>
      </div>
    </div>
    <div class="apply-now">
      Bewirb dich
      <a href="https://www.renuo.ch/en/jobs/ims-internship-2021-2022">jetzt</a>
    </div>
  </div>
</template>
<script>
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import Vue from "vue";
import internship_book from "@/assets/internship_book.jpeg";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";
Vue.use(BootstrapVue);
Vue.use(IconsPlugin);
import Bubble from "./Bubble.vue";
import VueSweetalert2 from "vue-sweetalert2";
// If you don't need the styles, do not connect
import "sweetalert2/dist/sweetalert2.min.css";
Vue.use(VueSweetalert2);

export default {
  name: "Internship",
  components: {
    Bubble
  },
  data() {
    return {
      internship_book: internship_book
    };
  },
  methods: {
    showEinfuehrung() {
      this.$swal(
        "Du wirst von den Mitarbeitern von Renuo in das Praktikum eingearbeitet und folgst einem detailierten Plan"
      );
    },
    showKundenprojekt() {
      this.$swal(
        "Du arbeitest an einem eigenen Projekt und erzeugst Mehrwert fuer einen Kunden. Du wirst waehrend dem Projekt vom Team unterstuetzt"
      );
    },
    showCoding() {
      this.$swal(
        "Nun wird endlich Software entwickelt. Bleib dran und erfreue dich an der Hauptaufgabe deines Praktikums"
      );
    },
    showIPA() {
      this.$swal(
        "Der Abschluss der Schulischen Aufgaben. Bei Renuo unterstuetzten wird dich eine gute Note zu erreichen"
      );
    },
    showStudium() {
      this.$swal(
        "Als Informatiker ist ein dauerhaftes weiterbilden eine wichtige Komponente von Erfolg. Also ab ins Studium"
      );
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
  width: 130%;
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
.ul--jobs-detail {
  padding-right: 50px;
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
  background-image: url("http://renuo.ch/images/header-gray-c059a3ec41d8322d3e3fa1656b578ccb.svg?vsn=d");
}

@media (max-width: 1200px) {
  .apply-now {
    font-size: 2.5vw;
  }
}

@media (max-width: 500px) {
  .apply-now {
    font-size: 4.5vw;
  }
}
</style>
