<template>
  <div class="instagram-grid" ref="instagram-grid">
    <img
      v-for="index in 25"
      :key="index"
      :src="require(`@/assets/instagram/image-${index}.jpeg`)"
    />
  </div>
</template>

<script>
export default {
  name: "Instagram.vue"
};
</script>

<style scoped lang="scss">
div.instagram-grid {
  width: 90%;
  margin: 0 auto;
  aspect-ratio: 1;
  display: grid;
  grid-column-gap: 2%;
  grid-row-gap: 2%;
  grid-template-rows: repeat(5, 18.4%);
  grid-template-columns: repeat(5, 18.4%);
  img {
    width: 100%;
    aspect-ratio: 1;
    opacity: 40%;
    transition: all 0.75s ease-in-out;
    &:hover {
      opacity: 100%;
      transition: all 50ms ease-in-out;
    }
  }
}
</style>
