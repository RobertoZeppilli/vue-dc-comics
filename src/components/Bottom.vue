<template>
  <div class="footer-bottom">
    <div class="container">
      <div class="button-container">
        <button>sign-up now!</button>
      </div>

      <div class="socials">
        <h3>follow us</h3>
        <div class="social-container">
          <a href="">
            <img src="../assets/img/footer-facebook.png" alt="facebook" />
          </a>
        </div>
        <div class="social-container">
          <a href="">
            <img src="../assets/img/footer-twitter.png" alt="twitter" />
          </a>
        </div>
        <div class="social-container">
          <a href="">
            <img src="../assets/img/footer-youtube.png" alt="youtube" />
          </a>
        </div>
        <div class="social-container">
          <a href="">
            <img src="../assets/img/footer-pinterest.png" alt="pinterest" />
          </a>
        </div>
        <div class="social-container">
          <a href="#">
            <img src="../assets/img/footer-periscope.png" alt="periscope" />
          </a>
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

.container {
    @include flexBetween;
    width: $containerWidth;
}

.footer-bottom {
  padding: 30px 0;
  background-color: #303030;
  @include flexBetween;
}

.socials {
  display: flex;
  align-items: center;
  h3 {
    text-transform: uppercase;
    color: $textColor;
    margin-right: 20px;
  }
  img {
    overflow: hidden;
    border-radius: 50%;
    &:hover {
      background-color: rgba($linkColor, 0.2); 
    }
  }
   
}

.social-container {
  margin-left: 0.7rem;
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