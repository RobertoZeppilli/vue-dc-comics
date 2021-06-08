<template>
  <div class="jumbotron">
      <span>Current Series</span>
  </div>
</template>

<script>
export default {
  name: "Jumbotron",
};
</script>

<style lang="scss" scoped>
@import '../style/variables';

.jumbotron {
    position: relative;
  height: 300px;
  width: 100%;
  background-image: url("../assets/img/jumbotron.jpg");
  background-size: cover;
}

span {
    position: absolute;
    background-color: $textColor;
}
</style>