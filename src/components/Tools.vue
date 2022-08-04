<template>
  <h2 class="h3-title">Tools</h2>
  <p>Mit diesen Werkzeugen arbeiten wir</p>
  <img class="img-fluid" alt="tools" :src="tools" />
  <h2 class="h3-title">Standort</h2>
  <p>Hier findest du uns</p>
  <div class="map img-fluid iframe-container">
    <iframe
      class="img-fluid remove-border"
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d219721.87235802517!2d8.508321660161725!3d47.35673387013604!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47900b1b31f3d935%3A0x4ac272717f6e976!2sRenuo%20AG!5e0!3m2!1sen!2sch!4v1597845570738!5m2!1sen!2sch"
      height="100%"
      width="80%"
      allowfullscreen=""
      aria-hidden="false"
      tabindex="0"
    ></iframe>
</template>

<script>
export default {
  name: "Tools"
};
</script>

<style scoped>

</style>
