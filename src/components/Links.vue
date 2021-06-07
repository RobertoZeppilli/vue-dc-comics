<template>
  <div class="belt">
    <div class="container">
      <div class="links-container">
        <div class="link">
          <img
            src="../assets/img/buy-comics-digital-comics.png"
            alt="digital-comics"
          />
          <h5>digital comics</h5>
        </div>
        <div class="link">
          <img
            src="../assets/img/buy-comics-merchandise.png"
            alt="merchandise"
          />
          <h5>dc merchandise</h5>
        </div>
        <div class="link">
          <img src="../assets/img/buy-comics-subscriptions.png" alt="sub" />
          <h5>subscription</h5>
        </div>
        <div class="link">
          <img
            class="shop"
            src="../assets/img/buy-comics-shop-locator.png"
            alt="shop-locator"
          />
          <h5>comic shop locator</h5>
        </div>
        <div class="link">
          <img
            class="svg"
            src="../assets/img/buy-dc-power-visa.svg"
            alt="visa"
          />
          <h5>dc power visa</h5>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Links",
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
  color: #fff;
}
.belt {
  height: 150px;
  background-color: #0282f9;
}

.svg {
  height: 90px;
}
</style>