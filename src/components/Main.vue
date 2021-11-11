<template>
  <main>
    <div class="bg-content">
      <div class="main-container">
        <h1>--Content goes here--</h1>
      </div>
    </div>

    <div class="bg-navbar2">
      <div class="main-container">
        <ul>
          <li v-for="(item, i) in navBarSecondary" :key="i">
            <img :src="item.img" alt="item.text" />
            <a href="#">{{ item.text }}</a>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "Main",
  data() {
    return {
      navBarSecondary: [
        {
          text: "Digital comics",
          href: "#",
          img: require("../assets/buy-comics-digital-comics.png"),
        },
        {
          text: "Dc merchandise",
          href: "#",
          img: require("../assets/buy-comics-merchandise.png"),
        },
        {
          text: "subscription",
          href: "#",
          img: require("../assets/buy-comics-subscriptions.png"),
        },
        {
          text: "comic shop location",
          href: "#",
          img: require("../assets/buy-comics-shop-locator.png"),
        },
        {
          text: "Dc power Visa",
          href: "#",
          img: require("../assets/buy-dc-power-visa.svg"),
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.bg-content {
  background-color: #1c1c1c;
}
.bg-navbar2 {
  background-color: #0282f9;
  ul {
    display: flex;
    justify-content: space-around;
    align-items: center;
    list-style-type: none;

    padding: 20px;
    img {
      width: 35px;
      vertical-align: middle;
    }
    a {
      color: white;
      text-decoration: none;
      text-transform: uppercase;
      padding-left: 10px;
      white-space: nowrap;
      font-size: 14px;
    }
  }
}
.main-container {
  width: 960px;
  margin: auto;
  h1 {
    color: white;
    margin: 0;
    padding: 20px;
  }
}
</style>