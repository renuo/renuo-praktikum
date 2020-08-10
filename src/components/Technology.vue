<template>
  <div>
    <div class="carousel-item" :class="isActive">
      <img :src="this.image" />
      <div class="carousel-caption d-none d-md-block">
        <h5>{{ this.technology }}</h5>
        <p>TEST</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Technologie",
  props: {
    technology: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    },
    active: {
      type: Boolean,
      required: true
    }
  },
  computed: {
    isActive() {
      if (this.active) {
        return "active";
      } else {
        return "";
      }
    }
  }
};
</script>
<style scoped lang="scss"></style>
