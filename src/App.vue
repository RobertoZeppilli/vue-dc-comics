<template>
  <div id="app">
    <Header />

    <main>
      <div class="container">
        <Content />
      </div>
    </main>
    <Links />

    <footer>
      <div class="container">
        <Dc />
      </div>
      <div class="footer-bottom">
        <Bottom />
      </div>
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header";
import Content from "./components/Content.vue";
import Links from "./components/Links";
import Dc from "./components/Dc";
import Bottom from "./components/Bottom.vue";

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
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

main {
  text-align: center;
  height: 100px;
  background-color: #191919;
}

footer {
  background-image: url(./assets/img/footer-bg.jpg);
  height: 300px;
}

.footer-bottom {
  background-color: #303030;
}
</style>
