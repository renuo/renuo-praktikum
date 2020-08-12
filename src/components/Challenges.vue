<template>
  <div class="hello">
    <h3>Unterfordert?</h3>

    <p>-</p>
  </div>
</template>

<script>
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

<style scoped>
h3 {
  margin: 4rem 20% 2px 20%;
  font-size: 2rem;
  color: #27d79d;
  font-weight: bold;

  border-width: 1px;
  border-color: black;
  border-style: none none solid none;
}

ul {
  list-style-type: none;
  padding: 0;
}

h2 {
  margin-top: 1.5rem;
  font-size: 2rem;
}

.values-img {
  margin: 1rem;
  size: 6rem 6rem !important;
  height: 3rem;
}

a {
  color: #42b983;
  font-size: 1rem;
}

p {
  margin-bottom: 10px;
}

.img-col {
  max-width: 15rem;
}

.col-md-6 {
  padding: 0px;
  width: 10rem;
}

.my-container {
  width: 80%;
  margin-left: auto;
  margin-right: auto;
}

.max-width {
  max-width: 60%;
}

.remove-border {
  border-style: none;
  border: 0;
}

@media only screen and (max-width: 1200px) {
  .smallFullSize {
    width: 100% !important;
  }
  .max-width {
    max-width: 100% !important;
  }
  .my-container {
    width: 100% !important;
  }
}
</style>
