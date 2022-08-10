<template>
  <div>
    <h2 ref="title">Please add a "title" prop</h2>
    <ul ref="list"></ul>
  </div>
</template>

<script>
import Vue from "vue";
import ChecklistItem from "@/components/ChecklistItem";

export default {
  name: "Checklist",
  props: ["title", "list"],
  mounted() {
    this.$refs.title.innerText = this.$props.title;
    const ComponentClass = Vue.extend(ChecklistItem);
    this.$props.list.forEach(text => {
      let instance = new ComponentClass();
      instance.$props["content"] = text;
      instance.$mount();
      this.$refs.list.appendChild(instance.$el);
    });
  }
};
</script>

<style scoped lang="scss">
@use "@/stylesheets/global.scss";
</style>
