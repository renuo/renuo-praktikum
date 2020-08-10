<template>
  <div>
    <div class="project_list">
      <li v-for="project in this.projects.projects" :key="project.title">
        <Project
          :title="project.title"
          :images="project.images"
          :description="project.description"
          :imgpos="project.imgpos"
          :technologies="project.technologies"
        />
      </li>
    </div>
  </div>
</template>

<script>
import json from "../json/projects.json";
import Project from "./Project.vue";
export default {
  name: "Projects",
  components: {
    Project
  },
  data: function() {
    return {
      projects: json
    };
  }
};
</script>
<style scoped lang="scss">
.project_list {
  width: 100%;
  list-style: none;
  li {
    padding-bottom: 5%;
  }
}
</style>
