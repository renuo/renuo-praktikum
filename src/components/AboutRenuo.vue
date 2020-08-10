<template>
  <div class="hello">
    <h1>About Renuo</h1>
    <h3>Team</h3>
    <img
      class="smallFullSize"
      style="width: 80%;"
      alt="technologies"
      src="assets/team.jpg"
    />
    <h3>Values</h3>
    <ul>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right">
              <img
                class="valuesIMG"
                alt="Quality and Precision"
                src="assets/w1.svg"
              />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">Quality and Precision</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right">
              <img
                class="valuesIMG"
                alt="Fairness and Transparency"
                src="assets/w2.svg"
              />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">Responsibility</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right">
              <img class="valuesIMG" alt="Responsibility" src="assets/w3.svg" />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">Responsibility</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right">
              <img class="valuesIMG" alt="Together" src="assets/w4.svg" />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">Together</h2>
            </div>
          </div>
        </div>
      </li>
      <li>
        <div class="container">
          <div class="row text-center">
            <div class="col-md-6 text-right">
              <img class="valuesIMG" alt="New ways" src="assets/w5.svg" />
            </div>
            <div class="col-md-6 text-left">
              <h2 class="">New ways</h2>
            </div>
          </div>
        </div>
      </li>
    </ul>
    <h3>Tools</h3>
    <img
      class="smallFullSize"
      style="width: 80%;"
      alt="technologies"
      src="assets/technologies.png"
    />
    <h3>Wo?</h3>
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
    <h3>Social media</h3>
    <ul>
      <li><a href="https://www.renuo.ch/">website</a></li>
      <li><a href="https://www.instagram.com/renuo_ag/">insta</a></li>
      <!--
      <li><a href="https://www.facebook.com/RenuoAG/">facebook</a></li>
      <li><a href="https://twitter.com/renuo">twitter</a></li>
      <li><a href="https://www.linkedin.com/authwall?trk=gf&trkInfo=AQETp1CcbNXcWQAAAXO5xE7ICqlVdf45_Qajp_xvrIr_eynm44xXPnzTsJx3SLdtoRFrA1pDZqeLIIHYSpFXfj-FFlpKwTIKWG-51OJD0QVXDXJbleYNoN3_f_gZvDGzLZq6haA=&originalReferer=https://www.renuo.ch/&sessionRedirect=https%3A%2F%2Fwww.linkedin.com%2Fcompany%2Frenuo">linkedin</a></li>
      <li><a href="https://www.xing.com/companies/renuoag">xing</a></li>
      <li><a href="https://github.com/renuo/">github</a></li>
      <li>email</li>
      -->
    </ul>
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
  margin: 2rem 0rem 0rem;
  font-size: 2rem;
}
ul {
  list-style-type: none;
  padding: 0;
}

.valuesIMG {
  margin: 1rem;
  width: 3rem;
  height: 3rem;
}

h2 {
  margin-top: 1.5rem;
  font-size: 1.5rem;
}

.col-md-6 {
  padding: 0px;
  width: 10rem;
}

a {
  color: #42b983;
  font-size: 1rem;
}

@media only screen and (max-width: 600px) {
  .smallFullSize {
    width: 100% !important;
  }
}
</style>
