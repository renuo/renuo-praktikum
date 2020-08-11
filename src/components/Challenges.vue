<template>
  <div class="hello">
    <h3>Unterfordert?</h3>
    <div style="width: 70%; margin: auto" class="smallFullSize">
        <p>Finde die längste wiederholende Teilzeichenkette in einem bestimmten Text.
            <ul>
                <li>Wiederholte Zeichenfolgen dürfen sich nicht überlappen. </li>
                <li>Wenn mehr als eine Zeichenkette mit gleicher Länge wiederholt wird, nimm die erste, die Du findest (beginnend mit dem Anfang des Textes).  </li>
            </ul>
            <b>Hinweis: </b>Leerzeichen gehören nicht zur Zeichenkette
        </p>
    </div>
  </div>
</template>

<script>
// eslint-disable-next-line no-unused-vars
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

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
  margin: 0rem;
  margin-top: 2rem;
  font-size: 2rem;
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

li, p{
    text-align: left;
}

p{
    margin-left: 1rem;
    margin-right: 1rem;
    font-size: 1rem;
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
  .smallFullSize{
    width: 100% !important;
  }
}

</style>
