<template>
  <div class="card">
    <img :src="item.thumb" :alt="item.series" />
    <p>{{ item.series }}</p>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["item"],
};
</script>

<style lang="scss" scoped>
@import "../style/variables";

.card {
  width: calc(100% / 6 - 20px);
  height: 150px;
  margin: 0 10px 60px 10px;

  & > img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top;
  }
}
p {
  color: $lightText;
  font-size: 0.7rem;
  font-weight: bold;
}
</style>