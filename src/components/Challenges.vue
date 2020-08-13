<template>
  <div class="hello">
    <h3 class="h3-title">Unterfordert?</h3>
  </div>
</template>

<script>
import "@/stylesheets/janis_css.css";

export default {
  name: "Challenges",
  props: {
    msg: String
  },
  data() {
    return {
      hover: false
    };
  }
};
</script>
