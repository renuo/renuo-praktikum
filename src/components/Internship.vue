<template>
  <div>
    <CenterTitle id="internship" title="Dein künftiger Praktikumsort" />
    <Notice />
    <img
      class="img-fluid"
      alt="Workspace"
      src="@/assets/about_renuo/work_space.png"
    />
    <Timeline
      class="timeline-center"
      :timeline-items="timelineItems"
      :colorDots="colorDots"
      :dateLocale="dateLocale"
      :shortToYearFormat="shortToYearFormat"
    />

    <Checklist class="mt-4" :list="checklistItems" />
  </div>
</template>
<script>
import "timeline-vuejs/dist/timeline-vuejs.css";
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import Vue from "vue";
import { BootstrapVue, IconsPlugin } from "bootstrap-vue";

Vue.use(BootstrapVue);
Vue.use(IconsPlugin);
import CenterTitle from "@/components/CenterTitle";
import Timeline from "@/components/Timeline";
import Checklist from "@/components/Checklist";
import Notice from "@/components/Notice";

let now = new Date();
let current_year = now.getFullYear();
if (now.getMonth() < 7) {
  current_year = current_year - 1;
}
export default {
  name: "Internship",
  components: {
    Checklist,
    Timeline,
    CenterTitle,
    Notice
  },
  data: () => ({
    dateLocale: "de-DE",
    shortToYearFormat: false,
    checklistItems: [
      "Softwareentwicklung mit Webtechnologien wie <a href='https://rubyonrails.org/' target='_blank'>Ruby on Rails</a>, <a href='https://angular.io/' target='_blank'>Angular</a>, <a href='https://reactjs.org/' target='_blank'>React</a>, HTML 5, Javascript und vielen mehr",
      "Anforderungsanalyse, technische Betreuung und Beratung von Kunden",
      "Datenbankdesign mit SQL (MySql, Postgres)",
      "Mitwirkung im Projektmanagement mit Scrum"
    ],
    timelineItems: [
      {
        from: new Date(current_year + 1, 7),
        title: "Einführung",
        description:
          "Du wirst von den Mitarbeitenden der Renuo ins Praktikum eingearbeitet und folgst einem detaillierten <a href='https://praktikumskonzept.renuo.ch' target='_blank'>Plan</a>."
      },
      {
        from: new Date(current_year + 1, 8),
        title: "Kundenprojekt",
        description:
          "Du arbeitest an einem eigenen Projekt und erzeugst Mehrwert für unsere Kundschaft. Du wirst während dem Projekt vom ganzen Team unterstützt."
      },
      {
        from: new Date(current_year + 1, 9),
        to: new Date(current_year + 2, 2),
        isMainTimeEntry: true,
        mainItemStyles: "background-color: #28d79d7d",
        title: "Coden",
        description:
          "Nun wird endlich Software entwickelt. Bleib dran und erfreue dich an der Hauptaufgabe deines Praktikums."
      },
      {
        from: new Date(current_year + 2, 2),
        title: "IPA (5+)",
        description:
          "Der Abschluss der schulischen Aufgaben. Bei der Renuo unterstützen wir dich, eine gute Note zu erreichen."
      },
      {
        from: new Date(current_year + 2, 8),
        title: "Studium (Arbeiten)",
        description:
          "Nach deinem Praktikum hast du die Möglichkeit, ein Studium zu beginnen und/oder weiter bei uns zu arbeiten."
      }
    ]
  })
};
</script>
<style lang="scss" scoped>
@use "@/stylesheets/global.scss";
@use "@/stylesheets/variables.scss";

.centered-gallery-image {
  z-index: 1;
  position: relative;
  width: 40%;
  border-radius: 10px;
  margin: auto;
}

.job-desc {
  margin-bottom: 0.5rem;
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
  margin-top: -50px;
  z-index: -1;
}

.ul--jobs-detail {
  list-style-image: url(https://www.renuo.ch/images/check-ddee0b6009fa00fff3365f0a93ccefb3.png?vsn=d);

  li {
    display: list-item;
    text-align: left !important;
    line-height: 1rem;

    a {
      font-weight: 200;
      padding-bottom: 0.25rem;
      border-bottom: 1px solid variables.$renuo-base-color;
      color: variables.$renuo-base-color;
      transition: all 0.5s;
    }
  }
}

.swal2-show {
  font-size: 2rem;
}

.apply-now {
  font-size: 1.5vw;
  background-color: variables.$renuo-base-color;
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
</style>
