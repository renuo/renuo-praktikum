<template>
  <li><span v-html="content"></span></li>
</template>

<script>
export default {
  name: "ChecklistItem",
  props: {
    content: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped lang="scss">
@use "@/stylesheets/global.scss";
@use "@/stylesheets/variables.scss";

li {
  list-style-type: none;
  margin-bottom: 5px;

  &:before {
    font-family: "Font Awesome 5 Pro";
    font-weight: 900;
    content: "\f00c";
    display: inline-block;
    color: variables.$renuo-base-color;
    margin-left: -1.3em;
    width: 1.3em;
  }

  i {
    margin-right: 5px;
    color: variables.$renuo-base-color;
  }
}
</style>
