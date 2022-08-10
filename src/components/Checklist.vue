<template>
  <div>
    <ul>
      <ChecklistItem :content="item" v-for="item in list" :key="item" />
    </ul>
  </div>
</template>

<script>
import ChecklistItem from "@/components/ChecklistItem";

export default {
  name: "Checklist",
  components: {
    ChecklistItem
  },
  props: {
    list: {
      type: Array,
      required: true
    }
  }
};
</script>

<style scoped lang="scss">
@use "@/stylesheets/global.scss";

div {
  max-width: 500px;
  margin: 0 auto;
}
</style>
