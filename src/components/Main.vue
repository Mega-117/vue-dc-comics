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
          <li>
            <img src="../assets/buy-comics-digital-comics.png" alt="" />
            <a href="#">Digital comics</a>
          </li>
          <li>
            <img src="../assets/buy-comics-digital-comics.png" alt="" />
            <a href="#">Digital comics</a>
          </li>
          <li>
            <img src="../assets/buy-comics-digital-comics.png" alt="" />
            <a href="#">Digital comics</a>
          </li>
          <li>
            <img src="../assets/buy-comics-digital-comics.png" alt="" />
            <a href="#">Digital comics</a>
          </li>
          <li>
            <img src="../assets/buy-comics-digital-comics.png" alt="" />
            <a href="#">Digital comics</a>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "Main",
  date() {
    return {
      navBar2: [
        {
          title: "Digital comics",
          href: "#",
          imgSrc: "buy-comics-digital-comics.png",
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
    list-style-type: none;
    margin: 0;
    padding: 20px;
    img {
      width: 40px;
      vertical-align: middle;
    }
    a {
      padding-left: 15px;
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