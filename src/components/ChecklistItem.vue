<template>
  <li><i class="fas fa-check"></i><span v-html="content"></span></li>
</template>

<script>
export default {
  name: "ChecklistItem",
  props: ["content"]
};
</script>

<style scoped lang="scss">
@use "@/stylesheets/global.scss";
@use "@/stylesheets/variables.scss";

li {
  list-style-type: none;
  i {
    margin-right: 5px;
    color: variables.$renuo-base-color;
  }
}
</style>
