<template>
  <div class="card">
    <img :src="item.thumb" :alt="item.series" />
    <p>{{ item.series }}</p>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["item"]
};
</script>

<style lang="scss" scoped>
@import "../style/variables";

.card {
  width: calc(100% / 6);
  padding: 0 10px;
  margin-bottom: 10px;

  & > img {
    width: 100%;
  }
}
p {
  color: #fff;
  font-size: .7rem;
  font-weight: bold;
}
</style>