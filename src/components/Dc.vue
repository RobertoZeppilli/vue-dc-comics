<template>
  <div class="container">
    <div class="footer-top">
      <div class="list-container">
        <ul class="list first-col">
          <li>
            <h4>dc comics</h4>
          </li>
          <li>
            <a href="#">Characters</a>
          </li>
          <li>
            <a href="#">Comics</a>
          </li>
          <li>
            <a href="#">Movies</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">Games</a>
          </li>
          <li>
            <a href="#">Videos</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
        </ul>
        <ul class="list second-col">
          <li>
            <h4>shop</h4>
          </li>
          <li>
            <a href="#">Shop DC</a>
          </li>
          <li>
            <a href="#">Shop DC Collectibles</a>
          </li>
        </ul>
      </div>
      <div class="list-container">
        <ul class="list third col">
          <li>
            <h4>dc</h4>
          </li>
          <li>
            <a href="#">Terms Of Use</a>
          </li>
          <li>
            <a href="#">Privacy policy (New)</a>
          </li>
          <li>
            <a href="#">Ad Choices</a>
          </li>
          <li>
            <a href="#">Advertising</a>
          </li>
          <li>
            <a href="#">Jobs</a>
          </li>
          <li>
            <a href="#">Subscriptions</a>
          </li>
          <li>
            <a href="#">Talent Workshops</a>
          </li>
          <li>
            <a href="#">CPSC Certificates</a>
          </li>
          <li>
            <a href="#">Ratings</a>
          </li>
          <li>
            <a href="#">Shop Help</a>
          </li>
          <li>
            <a href="#">Contact Us</a>
          </li>
        </ul>
      </div>
      <div class="list-container">
        <ul class="list fourth-col">
          <li>
            <h4>dc comics</h4>
          </li>
          <li>
            <a href="#">Characters</a>
          </li>
          <li>
            <a href="#">Comics</a>
          </li>
          <li>
            <a href="#">Movies</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">Games</a>
          </li>
          <li>
            <a href="#">Videos</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Dc",
};
</script>

<style lang="scss" scoped>
@import "../style/variables";

.footer-top {
  display: flex;
  padding: 30px 0;
  background-image: url(../assets/img/dc-logo-bg.png);
  background-size: 30rem auto;
  background-repeat: no-repeat;
  background-position: right center;
}
.list-container {
  margin-right: 25px;
}

.first-col {
  margin-bottom: 20px;
}
ul {
  list-style: none;

  li {
    color: #fff;
    text-transform: capitalize;
    a {
      color: $linkColor;
      text-decoration: none;
      font-size: 0.64rem;
      transition: color 0.5s ease-in-out;

      &:hover {
        color: $textColor;
      }
    }
  }
}
</style>