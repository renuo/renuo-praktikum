<template>
  <div>
    <h2>Tools</h2>
    <p class="subtitle">Mit diesen Werkzeugen arbeiten wir:</p>
    <div class="tools-listing">
      <a
        id="rails-run-spec-icon"
        href="https://github.com/rspec/rspec-rails"
        target="_blank"
        ><img alt="rails-run-spec-icon" src="@/assets/tools/rails-run-spec.png"
      /></a>
      <a id="git" href="https://git-scm.com/" target="_blank"
        ><img alt="git-icon" src="@/assets/tools/git.png"
      /></a>
      <a id="rails" href="https://rubyonrails.org/" target="_blank"
        ><img alt="rails-icon" src="@/assets/tools/rails.png"
      /></a>
      <a id="pytorch" href="https://pytorch.org/" target="_blank"
        ><img alt="pytorch-icon" src="@/assets/tools/pytorch.png"
      /></a>
      <a id="java" href="https://www.java.com/" target="_blank"
        ><img alt="java-icon" src="@/assets/tools/java.png"
      /></a>
      <a id="cloudflare" href="https://www.cloudflare.com/" target="_blank"
        ><img alt="cloudflare-icon" src="@/assets/tools/cloudflare.png"
      /></a>
      <a id="typescript" href="https://www.typescriptlang.org/" target="_blank"
        ><img alt="typescript-icon" src="@/assets/tools/typescript.png"
      /></a>
      <a id="scrum" href="https://www.scrum.org/" target="_blank"
        ><img alt="scrum-icon" src="@/assets/tools/scrum.png"
      /></a>
      <a id="ruby" href="https://www.ruby-lang.org/" target="_blank"
        ><img alt="ruby-icon" src="@/assets/tools/ruby.png"
      /></a>
      <a id="heroku" href="heroku.com" target="_blank"
        ><img alt="heroku-icon" src="@/assets/tools/heroku.png"
      /></a>
      <a id="sass" href="https://sass-lang.com/" target="_blank"
        ><img alt="sass-icon" src="@/assets/tools/sass.png"
      /></a>
      <a id="github" href="https://github.com/" target="_blank"
        ><img alt="github-icon" src="@/assets/tools/github.png"
      /></a>
      <a id="python" href="https://www.python.org/" target="_blank"
        ><img alt="python-icon" src="@/assets/tools/python.png"
      /></a>
      <a id="onepassword" href="https://1password.com/" target="_blank"
        ><img alt="onepassword-icon" src="@/assets/tools/onepassword.png"
      /></a>
      <a id="fork" href="https://git-fork.com/" target="_blank"
        ><img alt="fork-icon" src="@/assets/tools/fork.png"
      /></a>
      <a id="react" href="https://reactjs.org/" target="_blank"
        ><img alt="react-icon" src="@/assets/tools/react.png"
      /></a>
      <a id="slack" href="https://slack.com/" target="_blank"
        ><img alt="slack-icon" src="@/assets/tools/slack.png"
      /></a>
      <a id="aws" href="https://aws.amazon.com/" target="_blank"
        ><img alt="aws-icon" src="@/assets/tools/aws.png"
      /></a>
      <a id="vue" href="https://vuejs.org/" target="_blank"
        ><img alt="vue-icon" src="@/assets/tools/vue.png"
      /></a>
      <a id="apple" href="https://www.apple.com/" target="_blank"
        ><img alt="apple-icon" src="@/assets/tools/apple.png"
      /></a>
      <a id="jetbrains" href="https://www.jetbrains.com/" target="_blank"
        ><img alt="jetbrains-icon" src="@/assets/tools/jetbrains.png"
      /></a>
      <a id="semaphore" href="https://semaphoreci.com/" target="_blank"
        ><img alt="semaphore-icon" src="@/assets/tools/semaphore.png"
      /></a>
      <a
        id="m2"
        href="https://www.apple.com/chde/macbook-air-m2/"
        target="_blank"
        ><img alt="m2-icon" src="@/assets/tools/m2.png"
      /></a>
      <a id="webpack" href="https://webpack.js.org/" target="_blank"
        ><img alt="webpack-icon" src="@/assets/tools/webpack.png"
      /></a>
      <a id="osi" href="https://opensource.org/" target="_blank"
        ><img alt="osi-icon" src="@/assets/tools/osi.png"
      /></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Tools"
};
</script>

<style scoped lang="scss">
@use "@/stylesheets/global.scss";

div.tools-listing {
  width: 100%;
  aspect-ratio: 720/405;
  position: relative;
}

div.tools-listing a {
  position: absolute;
  display: block;
  transition: all 150ms ease-in-out;
}

div.tools-listing a:hover {
  transform: scale(1.1);
}

div.tools-listing a img {
  height: 100%;
  width: 100%;
}

a#git {
  width: 9%;
  aspect-ratio: 1;
  left: 11.25%;
  top: 24.7%;
}

a#rails-run-spec-icon {
  width: 12.5%;
  aspect-ratio: 1;
  left: 16%;
  top: 5.4%;
}

a#rails {
  aspect-ratio: 115/137;
  height: 33.9%;
  left: 38.4%;
  top: 19.4%;
}

a#pytorch {
  aspect-ratio: 1;
  height: 23.2%;
  left: 8.1%;
  top: 47.1%;
}

a#java {
  aspect-ratio: 1;
  height: 18.3%;
  left: 17.2%;
  top: 32.1%;
}

a#cloudflare {
  aspect-ratio: 88/53;
  height: 13.1%;
  left: 5.4%;
  top: 72%;
}

a#typescript {
  aspect-ratio: 1;
  height: 14.6%;
  left: 21%;
  top: 54.3%;
}

a#scrum {
  aspect-ratio: 1;
  height: 18.3%;
  left: 19.9%;
  top: 71.6%;
}

a#ruby {
  aspect-ratio: 64/56;
  height: 13.8%;
  top: 4.2%;
  left: 32.9%;
}

a#heroku {
  aspect-ratio: 1;
  height: 13.8%;
  left: 29%;
  top: 20.5%;
}

a#sass {
  aspect-ratio: 4/3;
  height: 11.1%;
  left: 30%;
  top: 39.5%;
}

a#github {
  aspect-ratio: 1;
  height: 39.8%;
  left: 29.2%;
  top: 49.4%;
}

a#slack {
  aspect-ratio: 1;
  height: 13.1%;
  left: 44.1%;
  top: 4.4%;
}

a#react {
  aspect-ratio: 115/81;
  height: 20%;
  left: 50%;
  top: 2%;
}

a#python {
  aspect-ratio: 1;
  height: 19%;
  left: 48.8%;
  top: 50.6%;
}

a#onepassword {
  aspect-ratio: 1;
  height: 28.4%;
  left: 46.5%;
  top: 68.6%;
}

a#jetbrains {
  aspect-ratio: 106/115;
  height: 27.4%;
  left: 54.6%;
  top: 23.3%;
}

a#fork {
  aspect-ratio: 1;
  height: 15.2%;
  left: 62.4%;
  top: 11.9%;
}

a#aws {
  aspect-ratio: 94/71;
  height: 17.5%;
  left: 71.7%;
  top: 2.2%;
}

a#vue {
  aspect-ratio: 77/67;
  height: 16.5%;
  left: 81.5%;
  top: 28.1%;
}

a#apple {
  aspect-ratio: 1;
  height: 38%;
  left: 61.2%;
  top: 38.3%;
}

a#semaphore {
  aspect-ratio: 1;
  height: 19%;
  left: 69.4%;
  top: 19.7%;
}

a#m2 {
  aspect-ratio: 1;
  height: 14.6%;
  left: 74.2%;
  top: 77.3%;
}

a#webpack {
  aspect-ratio: 1;
  height: 19%;
  left: 62.4%;
  top: 77%;
}

a#osi {
  aspect-ratio: 77/109;
  height: 26.9%;
  left: 81.3%;
  top: 45.4%;
}

p {
  text-align: center;
}
</style>
