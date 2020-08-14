<template>
  <div class="center-layout">
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
  </div>
</template>
<script>
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import Vue from "vue";

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

.center-layout {
  width: 60%;
  margin: auto;
}
.swal2-show {
  font-size: 2rem;
}
</style>
