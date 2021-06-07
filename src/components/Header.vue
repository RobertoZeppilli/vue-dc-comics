<template>
  <header>
    <div class="container">
      <a href="#logo">
        <img src="../assets/img/dc-logo.png" alt="logo" />
      </a>
      <nav>
        <ul>
          <li
            :class="link.active == true ? 'active' : ''"
            v-for="(link, index) in links"
            :key="index"
          >
            <a :href="link.url">
              {{ link.text }}
            </a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "characters",
          url: "#characters",
          active: false,
        },
        {
          text: "comics",
          url: "#comics",
          active: true,
        },
        {
          text: "movies",
          url: "#movies",
          active: false,
        },
        {
          text: "tv",
          url: "#tv",
          active: false,
        },
        {
          text: "games",
          url: "#games",
          active: false,
        },
        {
          text: "collectibles",
          url: "#colectibles",
          active: false,
        },
        {
          text: "videos",
          url: "#videos",
          active: false,
        },
        {
          text: "fans",
          url: "#fans",
          active: false,
        },
        {
          text: "news",
          url: "#news",
          active: false,
        },
        {
          text: "shop",
          url: "#shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.2rem;
  height: 100px;
}
img {
  width: 70%;
}

ul {
  display: flex;
  list-style: none;
  li {
    margin: 0 0.7rem;
    transition: all 0.5s ease-in-out;

    &.active,
    &:hover {
      border-bottom: 2px solid #0282f9;
    }
  }
  a {
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 0.7rem;
    color: #86847c;
    display: block;
    line-height: 98px;

    &:hover {
      color: #0282f9;
    }
  }
}
</style>