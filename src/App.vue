<template>
  <div id="app">
    <header>
      <Header />
      <Jumbotron />
    </header>
    <main>
      <Content />
      <Links />
    </main>
    <footer>
      <Dc />
      <Bottom />
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header";
import Jumbotron from './components/Jumbotron'
import Content from "./components/Content";
import Links from "./components/Links";
import Dc from "./components/Dc";
import Bottom from "./components/Bottom";

export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    Content,
    Links,
    Dc,
    Bottom,
  },
};
</script>

<style lang="scss">
@import "./style/variables";
@import './style/mixins';

* {
  @include reset;
  font-family: $font, sans-serif;
}
.container {
  max-width: $containerWidth;
  margin: 0 auto;
}

footer {
  background-image: url(./assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
