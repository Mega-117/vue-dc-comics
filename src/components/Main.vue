<template>
  <main>
    <div class="hero-container">
      <!-- <img src="../assets/jumbotron.jpg" alt="" /> -->
    </div>
    <div class="bg-content">
      <div class="main-container">
        <h1>--Content goes here--</h1>
        <div class="product-container">
          <ProductCard
            v-for="(product, i) in productsList"
            :key="i"
            :src="product.thumb"
            :prezzo="product.price"
            :serie="product.series"
            :tipo="product.type"
          ></ProductCard>
        </div>
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
import ProductCard from "@/components/ProductCard.vue";

export default {
  name: "Main",
  components: {
    ProductCard,
  },
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
      productsList: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.hero-container {
  height: 300px;
  background-image: url("../assets/jumbotron.jpg");
  background-size: cover;
  img {
    width: 100%;
  }
}
.bg-content {
  background-color: #1c1c1c;
}
.bg-navbar2 {
  background-color: #0282f9;
}
.main-container {
  width: 960px;
  margin: auto;
  .product-container {
    display: flex;
    flex-wrap: wrap;
  }

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
</style>