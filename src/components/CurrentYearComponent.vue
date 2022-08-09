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
      if (this.$props.augustchange === "true") {
        if (now.getMonth() >= 7) {
          return now.getFullYear() + parseInt(this.$props.increment);
        } else {
          return now.getFullYear() - 1 + parseInt(this.$props.increment);
        }
      } else {
        console.log(this.$props.augustchange);
        return now.getFullYear() + parseInt(this.$props.increment);
      }
    }
  }
};
</script>

<style scoped></style>
