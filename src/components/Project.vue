<template>
  <div>
    <div class="project_container">
      <div :class="getBackgroundContainerStyle" v-if="this.imgpos == 'left'">
        <div class="container">
          <div class="row">
            <div class="col-sm order-first">
              <ul class="image_list">
                <li v-for="image_source in this.images" :key="image_source">
                  <img class="side_image" :src="image_source" />
                </li>
              </ul>
            </div>
            <div class="col-sm text-side">
              <span :class="getTitleClass">{{ this.title }}</span>
              <br />
              <hr class="project_divider_renuo" />
              <div class="markdown-styling">
                <vue-markdown>
                  <template v-for="line in this.description">
                    {{ line }}
                  </template>
                </vue-markdown>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div :class="getBackgroundContainerStyle" v-else>
        <div class="container">
          <div class="row">
            <div class="col-sm text-side">
              <span :class="getTitleClass">{{ this.title }}</span>
              <br />
              <hr class="project_divider" />
              <div class="markdown-styling">
                <vue-markdown>
                  <template v-for="line in this.description">
                    {{ line }}
                  </template>
                </vue-markdown>
              </div>
            </div>
            <div class="col-sm order-first">
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
.side_image {
  width: 80%;
  margin-bottom: 2%;
  max-height: 10%;
  margin-left: auto;
  margin-right: auto;
  display: block;
}
.project_container {
  img:hover {
    transform: scale(1.1);
  }
}
.markdown-styling {
  text-align: left;
}
img {
  border-radius: 5px;
}

.text-side {
  ul {
    list-style: square outside !important;
  }
  p {
    text-align: left;
  }
}

.image_list {
  text-decoration: none;
  list-style: none;
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
  @include project_default_divider color: #27d79d;
}

.project_divider_renuo {
  @include project_default_divider;
}

.project_container {
  text-align: center;
}
</style>
