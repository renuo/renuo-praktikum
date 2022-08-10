<template>
  <div class="hello">
    <CenterTitle id="challenges" title="Challenge" />

    <div>
      <p class="mx-4">
        Die Teilnahme ist keine Voraussetzung für eine Bewerbung und nur zum
        Spass gedacht 🥳
      </p>
      <div class="corner-container">
        <a
          href="https://github.com/renuo/nearest-vowel"
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
    class Searcher
      VOWELS = # Add your code here

      def nearest_vowel(str)
        # Add your code here
        # Make sure that your solution is being returned
      end
    end
    </code></pre>
      </div>
      <p class="mx-4">
        Du kannst deine Lösung per Pull Request einreichen.
      </p>

      <p class="mx-4">
        Fragen kannst du im
        <a href="https://github.com/renuo/nearest-vowel/issues">Issues</a>
        Tab stellen.
      </p>

      <p class="mx-4">
        Das Projekt basiert auf einem einfachem Ruby script, sowie RSpec tests.
        Den Algorithmus musst du selbst schreiben, doch die Tests dazu sind
        bereits auf dem GitHub des Projektes unter dem «spec» Ordner.
      </p>

      <h2 class="mt-3 mb-2">Aufgabe</h2>

      <p class="mx-4">
        Deine Aufgabe ist es, die vorgegebene Funktion auszubauen, sodass sie
        mit einem eingegebenen String einen Array zurückgibt, welcher die
        Distanz von jedem Buchstaben zum nächsten Vokal zeigt. Das würde dann
        wie folgt aussehen:
      </p>

      <pre><code class="language-ruby code-display">
    Searcher.nearest_vowel("Renuo AG")
      </code></pre>

      <p class="mx-4">
        Die Funktion soll dann folgenden Array zurückgeben:
      </p>

      <pre><code class="language-ruby code-display">
    [1, 0, 1, 0, 0, 1, 0, 1]
      </code></pre>
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
@use "@/stylesheets/global.scss";
.corner-container {
  position: relative;
}

.github-corner {
  position: absolute;
  right: 0;
  top: 0;
}

.github-corner:hover .octo-arm {
  animation: octocat-wave 560ms ease-in-out;
}
@keyframes octocat-wave {
  0%,
  100% {
    transform: rotate(0);
  }
  20%,
  60% {
    transform: rotate(-25deg);
  }
  40%,
  80% {
    transform: rotate(10deg);
  }
}
</style>
