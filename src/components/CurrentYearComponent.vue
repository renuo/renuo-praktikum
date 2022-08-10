<template>
  <span>{{ currentYear() }}</span>
</template>

<script>
export default {
  name: "CurrentYearComponent",
  props: ["augustchange", "increment"],
  methods: {
    currentYear() {
      let now = new Date();
      if (this.$props.augustchange) {
        if (now.getMonth() >= 7) {
          return now.getFullYear() + this.$props.increment;
        } else {
          return now.getFullYear() - 1 + this.$props.increment;
        }
      } else {
        return now.getFullYear() + this.$props.increment;
      }
    }
  }
};
</script>

<style scoped></style>
