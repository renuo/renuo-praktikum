<template>
  <template>
    <img class="goodies-img-fluid" alt="goodies" :src="goodies" />
    <p>
      Komm zu uns, wir bieten dir nebst Coding-Erfahrung noch mehr Benefits.
      Lass Sie dir nicht entgehen.
    </p>
  </template>

  <script>
    export default {
      name: "Goodies",
      data() {
        return {
          goodies: goodies
        };
      }
    };
  </script>

  <style scoped></style>
</template>
