<template>
  <section class="belt">
    <div class="container">
      <div class="links-container">
        <div v-for="(link, index) in links" :key="index" class="link">
          <img
            :src="link.img"
            :alt="link.text"
            :class="{ 'svg' : link.svg == true, 'shop' : link.resize == true }"
          />
          <h5>{{ link.text }}</h5>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Links",
  data() {
    return {
      links: [
        {
          text: "digital comics",
          img: require("../assets/img/buy-comics-digital-comics.png"),
          resize: false,
          svg: false
        },
        {
          text: "dc merchandise",
          img: require("../assets/img/buy-comics-merchandise.png"),
          resize: false,
          svg: false
        },
        {
          text: "subscriptions",
          img: require("../assets/img/buy-comics-subscriptions.png"),
          resize: false,
          svg: false
        },
        {
          text: "comic shop locator",
          img: require("../assets/img/buy-comics-shop-locator.png"),
          resize: true,
          svg: false
        },
        {
          text: "dc power visa",
          img: require("../assets/img/buy-dc-power-visa.svg"),
          resize: false,
          svg: true
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables";

.container {
  height: 100%;
  width: calc($containerWidth - 300px);
  margin: 0 auto;
}
.links-container {
  display: flex;
  height: 100%;
}
.link {
  display: flex;
  align-items: center;
  justify-content: center;
  img {
    width: 20%;
    margin-right: 10px;
    &.shop {
      width: 15%;
    }
  }
}

h5 {
  text-transform: uppercase;
  font-size: 0.7rem;
  color: #fff;
}
.belt {
  height: 150px;
  background-color: #0282f9;
}

.svg {
  height: 100px;
}
</style>