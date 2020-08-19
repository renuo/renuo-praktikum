<template>
  <div>
    <div class="project_container">
      <div :class="getBackgroundContainerStyle">
        <div class="content-container">
          <img class="heading-image" :src="images[0]" />
          <br />
          <br />
          <br />
          <span :class="getTitleClass">{{ this.title }}</span>
          <br />
          <hr class="project_divider_renuo" />
          <div class="markdown-styling">
            <vue-markdown>
              <template v-for="line in this.description">
                {{ line }}
              </template>
            </vue-markdown>
            <a :href="this.more">Mehr</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import VueMarkdown from "vue-markdown";

export default {
  name: "Project",
  props: {
    title: {
      type: String,
      required: true
    },
    more: {
      type: String,
      required: true
    },

    description: {
      type: Array,
      required: true
    },
    images: {
      type: Array,
      required: true
    },
    imgpos: {
      type: String,
      required: true
    },
    technologies: {
      type: Array,
      required: false
    }
  },
  components: {
    VueMarkdown
  },
  methods: {},
  computed: {
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
.project_container {
  img {
    width: 100%;
    max-height: auto;
    border-radius: 10px;
  }

  img:hover {
    transform: scale(1.1);
  }
}

@media only screen and (min-width: 700px) {
  .project_container {
    img {
      width: 80%;
      max-height: 600px;
      border-radius: 10px;
    }
  }
  .project_container {
    p {
      font-size: 3rem !important;
    }
  }
}

@media only screen and (min-width: 1000px) {
  .project_container {
    img {
      width: 60%;
      max-height: 800px;
      border-radius: 10px;
    }
  }
}

.content-container {
  width: 80%;
}

a {
  position: relative;
}

ul {
  list-style-type: square !important;
}

@mixin project_title_default {
  font-weight: bold;
  color: #143327;
  text-align: center;
  font-size: 3vw;
  line-height: 1.2;
  color: #27d79d;
  padding-bottom: 1%;
}

.project_title {
  @include project_title_default;
}

@mixin project_card_padding {
  padding-top: 2vw;
  padding-bottom: 2vw;
}

.project_container {
  background-color: #fff !important;
  padding-top: 2%;
  padding-bottom: 2%;
  @include project_card_padding;
}

.project_container_renuo {
  background-color: #27d79d !important;
  color: white;
  @include project_card_padding;
}
.project_title_white {
  @include project_title_default;
  color: #fff !important;
}

@mixin project_default_divider {
  width: 50%;
  margin-left: auto;
  margin-right: auto;
  color: white;
}

.project_divider {
  @include project_default_divider;
  color: #27d79d;
}

.project_divider_renuo {
  @include project_default_divider;
}

.project_container {
  text-align: center;
}
@media (max-width: 700px) {
  .project_title_white {
    font-size: 5vw;
  }
  .project_title {
    font-size: 5vw;
  }
}
</style>
