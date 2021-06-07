<template>
  <div id="app">
    <Header />
    <Content />
    <Links />

    <footer>
      <Dc />

      <Bottom />
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header";
import Content from "./components/Content";
import Links from "./components/Links";
import Dc from "./components/Dc";
import Bottom from "./components/Bottom";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Links,
    Dc,
    Bottom,
  },
};
</script>

<style lang="scss">

@import './style/variables';

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  max-width: $containerWidth;
  margin: 0 auto;
}

footer {
  background-image: url(./assets/img/footer-bg.jpg);
  height: 300px;
}
</style>
