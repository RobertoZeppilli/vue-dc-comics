<template>
  <div class="container">
    <div class="navigation">
      <div class="logo">
        <a href="#logo">
          <img src="../assets/img/dc-logo.png" alt="logo" />
        </a>
      </div>
      <nav>
        <ul>
          <li
            v-for="(link, index) in links"
            :key="index"
            @click="getActive(index)"
            :class="{ active: index == activeIndex }"
          >
            <a :href="link.url">
              {{ link.text }}
            </a>
          </li>
        </ul>
      </nav>
    </div>
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
          url: "#characters",
        },
        {
          text: "comics",
          url: "#comics",
        },
        {
          text: "movies",
          url: "#movies",
        },
        {
          text: "tv",
          url: "#tv",
        },
        {
          text: "games",
          url: "#games",
        },
        {
          text: "collectibles",
          url: "#colectibles",
        },
        {
          text: "videos",
          url: "#videos",
        },
        {
          text: "fans",
          url: "#fans",
        },
        {
          text: "news",
          url: "#news",
        },
        {
          text: "shop",
          url: "#shop",
        },
      ],
      activeIndex: 0,
    };
  },
  methods: {
    getActive: function (index) {
      return (this.activeIndex = index);
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables";
@import "../style/mixins";

.navigation {
  @include flex ($type: 'between');
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
    margin-left: 0.7rem;
    line-height: 96px;
    transition: all 0.5s ease-in-out;

    &.active,
    &:hover {
      border-bottom: 4px solid $textColor;
    }
  }
  a {
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 0.7rem;
    color: $linkColor;
    display: block;
    line-height: 96px;

    &:hover {
      color: $textColor;
    }
  }
}
</style>