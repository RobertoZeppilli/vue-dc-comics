<template>
  <div class="container">
    <header>
      <a href="#logo">
        <img src="../assets/img/dc-logo.png" alt="logo" />
      </a>
      <nav>
        <ul>
          <li
            v-for="(link, index) in links"
            :key="index"
            @click="getActive(index)"
            :class="{'active' : index == activeIndex}"
          >
            <a :href="link.url">
              {{ link.text }}
            </a>
          </li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "characters",
          url: "#characters"
        },
        {
          text: "comics",
          url: "#comics"
        },
        {
          text: "movies",
          url: "#movies"
        },
        {
          text: "tv",
          url: "#tv"
        },
        {
          text: "games",
          url: "#games"
        },
        {
          text: "collectibles",
          url: "#colectibles"
        },
        {
          text: "videos",
          url: "#videos"
        },
        {
          text: "fans",
          url: "#fans"
        },
        {
          text: "news",
          url: "#news"
        },
        {
          text: "shop",
          url: "#shop"
        },
      ],
      activeIndex: 0
    };
  },
  methods: {
    getActive: function (index) {
      return this.activeIndex = index
    }
  }
};
</script>

<style lang="scss" scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.2rem 0;
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
    padding: 0 0.5rem;
    transition: all 0.5s ease-in-out;

    &.active {
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