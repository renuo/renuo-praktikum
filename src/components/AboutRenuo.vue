<template>
  <div class="my-container">
    <h3 class="remove-border">Gemeinsam sind wir Renuo!</h3>
    <img class="img-full" alt="technologies" src="assets/team.jpg" />
    <h3>Fokus und Stärken</h3>
    <p>Wir entwickeln individuelle Software auf höchstem Niveau.</p>
    <ul>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img
                class="values-img"
                alt="Quality and Precision"
                src="assets/w1.svg"
              />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">Qualität und Präzision</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img
                class="values-img"
                alt="Fairness and Transparency"
                src="assets/w2.svg"
              />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">Verantwortlichkeit</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img
                class="values-img"
                alt="Responsibility"
                src="assets/w3.svg"
              />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">Gerechtigkeit und Transparenz</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img class="values-img" alt="Together" src="assets/w4.svg" />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">Neue Wege</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img class="values-img" alt="New ways" src="assets/w5.svg" />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">Zusammen</h2>
            </div>
          </div>
        </div>
      </li>
    </ul>
    <h3>Tools</h3>
    <p>Damit arbeiten wir</p>
    <img class="img-padded" alt="tools" src="assets/tools.png" />
    <h3>Standort</h3>
    <p>Hier findest du uns</p>
    <div class="map img-full">
      <iframe
        class="img-full remove-border"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2700.059992876826!2d8.588275315623724!3d47.41077097917222!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47900b1b31f3d935%3A0x4ac272717f6e976!2sRenuo%20AG!5e0!3m2!1sen!2sch!4v1596548442258!5m2!1sen!2sch"
        height="600rem"
        width="80%"
        allowfullscreen=""
        aria-hidden="false"
        tabindex="0"
      ></iframe>
      <img class="cat" :src="cat" />
    </div>
    <blockquote>
      Aa zelle Bölle schelle, d’Chatz gaht uf Walliselle
    </blockquote>
    <h3>Kundenauszug</h3>
    <p>
      Die Stärke der Renuo zeigt sich in der Vielseitigkeit der Produkte, welche
      von den verschiedensten Branchen und Firmen beauftragt wurden.
    </p>
    <img class="img-padded" alt="tools" src="assets/kundenauszug.png" />
  </div>
</template>

<script>
import cat from "@/assets/cat.png";
export default {
  name: "AboutRenuo",
  data() {
    return {
      cat: cat,
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

.img-padded {
  margin: 4%;
  width: 92%;
}

.img-full {
  width: 100%;
}

.remove-border {
  border-style: none;
  border: 0;
}

.map {
  position: relative;
}

@media only screen and (max-width: 1200px) {
  .my-container {
    width: 100% !important;
  }
}

.cat {
  width: 10rem;
  position: absolute;
  left: 0;
  bottom: 0;
}

blockquote {
  background: #f9f9f9;
  border-left: 10px solid #ccc;
  margin: 1.5em 10px;
  padding: 0.5em 10px;
  quotes: "\201C""\201D""\2018""\2019";
}
blockquote:before {
  color: #ccc;
  content: open-quote;
  font-size: 4em;
  line-height: 0.1em;
  margin-right: 0.25em;
  vertical-align: -0.4em;
}
blockquote p {
  display: inline;
}
</style>
