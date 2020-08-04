<template>
  <div class="hello">
    <h1>About Renuo</h1>

    <h3>Werte</h3>

    <v-container class="grey lighten-5">
      <v-row no-gutters>
        <v-col sm="5">
          <v-card class="pa-2" outlined>
            <img
              @mouseover="hover = true"
              @mouseleave="hover = false"
              alt="w"
              src="../assets/w1.svg"
            />

            <span v-if="hover">Quality and Precision</span>
          </v-card>
          <v-card class="pa-2" outlined>
            <img alt="Fairness and Transparency" src="../assets/w2.svg" />
          </v-card>

          <v-card class="pa-2" outlined>
            <img alt="Responsibilitz" src="../assets/w3.svg" />
          </v-card>

          <v-card class="pa-2" outlined>
            <img alt="Together" src="../assets/w4.svg" />
          </v-card>

          <v-card class="pa-2" outlined>
            <img alt="New ways" src="../assets/w5.svg" />
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <h3>Tools</h3>
    <h3>Wo?</h3>
    <h3>Social media</h3>
    <ul>
      <li>insta</li>
      <li />
      <li>website</li>
      <li />
      <li>email</li>
      <li />
    </ul>
  </div>
</template>

<script>

export default {
  name: 'AboutRenuo',
  props: {
    msg: String
  },
  data () {
    return {
      hover: false
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

img {
  width: 10%;
  height: 10%;
}
</style>
