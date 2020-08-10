<template>
  <div>
    <div :class="getBackgroundContainerStyle" v-if="this.imgpos == 'left'">
      <div class="container">
        <div class="row">
          <div class="col-sm">
            <ul class="image_list">
              <li v-for="image_source in this.images" :key="image_source">
                <img class="side_image" :src="image_source" />
              </li>
            </ul>
          </div>
          <div class="col-sm">
            <span :class="getTitleClass">{{ this.title }}</span>
            <br />
            <p v-html="this.description"></p>
          </div>
        </div>
      </div>
    </div>
    <div :class="getBackgroundContainerStyle" v-else>
      <div class="container">
        <div class="row">
          <div class="col-sm">
            <span class="project_title">{{ this.title }}</span>
            <br />
            <p v-html="this.description"></p>
          </div>
          <div class="col-sm">
            <ul class="image_list">
              <li v-for="image_source in this.images" :key="image_source">
                <img class="side_image" :src="image_source" />
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Project",
  props: {
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
    images: {
      type: Array,
      required: true
    },
    imgpos: {
      type: String,
      required: true
    }
  },
  methods: {
    getTitleClass() {
      if (this.imgpos == "left") {
        return "project_title";
      } else {
        return "project_title_white";
      }
    },
    getBackgroundContainerStyle() {
      if (this.imgpos == "left") {
        return "project_container";
      } else {
        return "project_container_renuo";
      }
    },
    getTextStyling() {
      return "";
    }
  }
};
</script>
<style scoped lang="scss">
.side_image {
  width: 50%;
  margin-bottom: 2%;
}
.image_list {
  text-decoration: none;
  list-style: none;
}
.project_title {
  font-weight: 500;
  color: #143327;
  text-align: center;
  font-size: 4rem;
  line-height: 1.2;
  color: #27d79d;
  padding-bottom: 1%;
}

.project_container {
  background-color: #fff !important;
}

.project_container_renuo {
  background-color: #27d79d !important;
}
.project_title_white {
  font-weight: 500;
  color: #143327;
  text-align: center;
  font-size: 4rem;
  line-height: 1.2;
  color: #fff;
  padding-bottom: 1%;
}
</style>
