<template>
  <div class="container">
    <div class="footer-bottom">
      <div class="button-container">
        <button>sign-up now!</button>
      </div>

      <div class="socials">
        <h3>follow us</h3>
        <div class="social-container">
          <img src="../assets/img/footer-facebook.png" alt="facebook" />
        </div>
        <div class="social-container">
          <img src="../assets/img/footer-twitter.png" alt="twitter" />
        </div>
        <div class="social-container">
          <img src="../assets/img/footer-youtube.png" alt="youtube" />
        </div>
        <div class="social-container">
          <img src="../assets/img/footer-pinterest.png" alt="pinterest" />
        </div>
        <div class="social-container">
          <img src="../assets/img/footer-periscope.png" alt="periscope" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Bottom",
};
</script>

<style lang="scss" scoped>

@import "../style/variables";

.footer-bottom {
  height: 100px;
  background-color: #303030;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.socials {
  display: flex;
  align-items: center;
  h3 {
    text-transform: uppercase;
    color: $textColor;
    margin-right: 20px;
  }
}

.social-container {
  margin: 0 10px;
}
button {
  background-color: transparent;
  outline: none;
  padding: 10px 20px;
  border: 1px solid $textColor;
  text-transform: uppercase;
  cursor: pointer;
  color: #fff;
  transition: background-color 0.5s ease-in-out;
}

button:hover {
  background-color: $textColor;
}
</style>