<template>
  <div>
    <h2 class="h3-title" id="about-renuo">Das Team</h2>
    <img class="img-fluid" alt="renuo team" :src="team" />
    <h2 class="h3-title">Goodies</h2>
    <p>
      Komm zu uns, wir bieten dir nebst Coding-Erfahrung noch mehr Benefits.
      Lass Sie dir nicht entgehen.
    </p>
    <div>
      <a href="https://renuo.ch/jobs" class="btn btn-info" role="button"
        >Komm zu uns ins Team</a
      >
    </div>
    <script>
      export default {
        name: "Team",
        data() {
          return {
            team: team
          };
        }
      };
    </script>

    <style scoped></style></div
></template>
