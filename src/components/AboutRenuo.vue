<template>
  <div class="hello">
    <h3 style="border-style: none;">Gemeinsam sind wir Renuo!</h3>
    <img
      class="smallFullSize"
      style="width: 80%;"
      alt="technologies"
      src="assets/team.jpg"
    />
    <h3>Fokus und Stärken</h3>
    <p>Wir entwickeln individuelle Software auf höchstem Niveau.</p>
    <ul>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right img-col">
              <img
                class="valuesIMG"
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
                class="valuesIMG"
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
              <img class="valuesIMG" alt="Responsibility" src="assets/w3.svg" />
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
              <img class="valuesIMG" alt="Together" src="assets/w4.svg" />
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
              <img class="valuesIMG" alt="New ways" src="assets/w5.svg" />
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
    <img
      class="smallFullSize"
      style="width: 80%;"
      alt="technologies"
      src="assets/tools.png"
    />

    <h3>Standort</h3>
    <p>Hier findest du uns</p>
    <iframe
      class="smallFullSize"
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2700.059992876826!2d8.588275315623724!3d47.41077097917222!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47900b1b31f3d935%3A0x4ac272717f6e976!2sRenuo%20AG!5e0!3m2!1sen!2sch!4v1596548442258!5m2!1sen!2sch"
      width="80%"
      height="400rem"
      style="border:0;"
      allowfullscreen=""
      aria-hidden="false"
      tabindex="0"
    ></iframe>

    <h3>Kundenauszug</h3>
    <p>
      Die Stärke der Renuo zeigt sich in der Vielseitigkeit der Produkte, welche
      von den verschiedensten Branchen und Firmen beauftragt wurden.
    </p>
    <img
      class="smallFullSize"
      style="width: 80%;"
      alt="tools"
      src="assets/kundenauszug.png"
    />
  </div>
</template>

<script>
export default {
  name: "AboutRenuo",
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

.valuesIMG {
  margin: 1rem;
  size: 6rem 6rem !important;
  height: 3rem;
}

h2 {
  margin-top: 1.5rem;
  font-size: 2rem;
}

.img-col {
  max-width: 15rem;
}

.col-md-6 {
  padding: 0px;
  width: 10rem;
}

a {
  color: #42b983;
  font-size: 1rem;
}

p {
  margin-bottom: 10px;
}

@media only screen and (max-width: 1200px) {
  .smallFullSize {
    width: 100% !important;
  }
}
</style>
