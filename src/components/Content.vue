<template>
  <section>
    <div class="container card-container">
      <Card :item="comic" v-for="(comic, index) in comics" :key="index" />
      <Button />
    </div>
  </section>
</template>

<script>
import Card from "../components/Card";
import Button from "../components/Button";
import comics from "../../JSON/dc-comics.json"
export default {
  name: "Content",
  components: {
    Card,
    Button,
  },
  data() {
    return {
      // file json
      comics,
      // file json
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables";
@import "../style/mixins";

section {
  background-color: $bgDark;
}
.card-container {
  background-color: $bgDark;
  @include flex($type: "center");
  flex-wrap: wrap;
  padding: 40px 0;
}
</style>