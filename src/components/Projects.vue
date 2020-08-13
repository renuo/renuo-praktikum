<template>
  <div>
    <div class="project_list">
      <li v-for="(project, index) in this.projects" :key="project.title">
        <Project
          :title="project.title"
          :images="project.images"
          :description="project.description"
          :imgpos="project.imgpos"
          :technologies="project.technologies"
        />
        <hr v-if="needsBreakbar(index)" />
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
  methods: {
    needsBreakbar(current_index) {
      if (current_index == 0 || current_index == this.projects.length - 1) {
        return false;
      } else if (
        !(
          this.projects[current_index + 1].imgpos ==
          this.projects[current_index].imgpos
        )
      ) {
        return false;
      } else {
        return true;
      }
    }
  },
  data: function() {
    return {
      projects: json.projects
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
