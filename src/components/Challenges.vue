<template>
  <div class="hello">
    <CenterTitle id="challenges" title="Challenge" />

    <div class="instructions">
      <h4 class="readme-title">Wir haben eine Challenge für dich!</h4>
      <p class="readme-text">
        <span style="color: red;">Achtung</span> Die Teilnahme ist keine
        Voraussetzung für eine Bewerbung und nur zum Spass gedacht.
      </p>
      <div class="corner-container" style="width: 100%;">
        <a
          href="https://github.com/renuo/christmas_tree"
          class="github-corner"
          aria-label="View source on GitHub"
          ><svg
            width="80"
            height="80"
            viewBox="0 0 250 250"
            style="fill:#151513; color:#fff; position: absolute; top: 0; border: 0; right: 0;"
            aria-hidden="true"
          >
            <path d="M0,0 L115,115 L130,115 L142,142 L250,250 L250,0 Z"></path>
            <path
              d="M128.3,109.0 C113.8,99.7 119.0,89.6 119.0,89.6 C122.0,82.7 120.5,78.6 120.5,78.6 C119.2,72.0 123.4,76.3 123.4,76.3 C127.3,80.9 125.5,87.3 125.5,87.3 C122.9,97.6 130.6,101.9 134.4,103.2"
              fill="currentColor"
              style="transform-origin: 130px 106px;"
              class="octo-arm"
            ></path>
            <path
              d="M115.0,115.0 C114.9,115.1 118.7,116.5 119.8,115.4 L133.7,101.6 C136.9,99.2 139.9,98.4 142.2,98.6 C133.8,88.0 127.5,74.4 143.8,58.0 C148.5,53.4 154.0,51.2 159.7,51.0 C160.3,49.4 163.2,43.6 171.4,40.1 C171.4,40.1 176.1,42.5 178.8,56.2 C183.1,58.6 187.2,61.8 190.9,65.4 C194.5,69.0 197.7,73.2 200.1,77.6 C213.8,80.2 216.3,84.9 216.3,84.9 C212.7,93.1 206.9,96.0 205.4,96.6 C205.1,102.4 203.0,107.8 198.3,112.5 C181.9,128.9 168.3,122.5 157.7,114.1 C157.9,116.9 156.7,120.9 152.7,124.9 L141.0,136.5 C139.8,137.7 141.6,141.9 141.8,141.8 Z"
              fill="currentColor"
              class="octo-body"
            ></path></svg
        ></a>
        <pre><code class="language-ruby code-display">
    # frozen_string_literal: true

    class ChristmasTree
      TREE_CHARACTER = 'X'

      def draw(height)
        # TODO: implement logic
        height
      end
    end
    </code></pre>
      </div>
      <p class="readme-text">
        Du kannst deine Lösung per Pull Request einreichen.
      </p>

      <p class="readme-text">
        Fragen kannst du im
        <a href="https://github.com/renuo/christmas_tree/issues">"Issues"</a>
        Tab stellen.
      </p>

      <h4 class="readme-title">Weihnachtsbaum 🌲</h4>

      <p class="readme-text">
        Obwohl es noch nicht Weihnachten ist, hoffen wir trotzdem, dass du Spass
        mit dieser Challenge haben wirst. 😎
      </p>

      <h4 class="readme-sub-title">Basis</h4>

      <p class="readme-text">
        Kleine ruby app mir bereits vorbereiteten tests..
      </p>

      <h4 class="readme-sub-title">Aufgabe</h4>

      <p class="readme-text">
        Du musst eine Funktion schreiben, welche einen Weihhnachtsbaum in ASCII
        art zurück gibt. Versuche test-driven (TDD) in Ruby zu entwicklen.
      </p>

      <h4 class="readme-sub-sub-title">Input</h4>

      <p class="readme-text">
        Deine Funktion sollte als ihren ersten Parameter die Höhe des Baumes
        annehmen.
      </p>

      <h4 class="readme-sub-sub-title">Output</h4>

      <p class="readme-text">
        Die implementierte Funktion sollte einen Weihnachtsbaum als string
        zurück geben.
      </p>

      <pre><code class="language-bash code-display">
    ChristmasTree.draw(5)
      </code></pre>

      <p class="readme-text">Der Output sollte dann wie folgt aussehen:</p>
      <pre><code class="language-bash code-display">
        X
       XXX
      XXXXX
     XXXXXXX
    XXXXXXXXX
      </code></pre>

      <h4 class="readme-sub-title">Fortgeschritten</h4>

      <p class="readme-text">
        Langsam nimmt der Baum Form an. Wenn du noch einen Schritt weiter gehen
        willst, kannst du dem Baum einen Stamm und einen Stern geben.
      </p>
      <p class="readme-text">
        Zusätzlich könntest du der Funktion zwei weiterere Argumente geben, die
        bestimmen ob der Baum einen Stamm beziehungsweise Stern haben soll.
      </p>
      <pre><code class="language-bash code-display">
    ChristmasTree.draw(height: 5, tree_stand: true, star: true)
      </code></pre>

      <p class="readme-text">
        Wenn beide Argumente auf `true` sind, sollte dies der ouput sein:
      </p>

      <pre><code class="language-bash code-display">
        *
        X
       XXX
      XXXXX
     XXXXXXX
    XXXXXXXXX
        |
      </code></pre>

      <p class="readme-text">
        Vergiss nicht einen Test für diese Aufgabe zu schreiben. 👨🏻‍💻 👩🏼‍💻
      </p>
    </div>
  </div>
</template>

<script>
import CenterTitle from "@/components/CenterTitle";

export default {
  name: "Challenges",
  components: {
    CenterTitle
  },
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

<style lang="scss" scoped>
@import "@/stylesheets/global.scss";
// todo: use https://highlightjs.org/
</style>
