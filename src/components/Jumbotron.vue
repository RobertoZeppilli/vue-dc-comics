<template>
  <div class="jumbotron">
    <div class="container">
      <h3>Current Series</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "Jumbotron",
};
</script>

<style lang="scss" scoped>
@import "../style/variables";

.jumbotron {
  position: relative;
  height: 300px;
  width: 100%;
  background-image: url("../assets/img/jumbotron.jpg");
  background-size: cover;
  h3 {
    position: absolute;
    bottom: -20px;
    background-color: $textColor;
    padding: 10px 20px;
    color: $lightText;
    text-transform: uppercase;
  }
}
</style>