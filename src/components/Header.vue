
<template>
  <div class="container">
    <header>
      <nav>
        <div class="logo-container">
          <img src="../assets/dc-logo.png" alt="" />
        </div>
        <ul>
          <li v-for="(item, i) in navBarItem" :key="i">
            <a :href="item.href">{{ item.title }}</a>
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
      navBarItem: [
        {
          title: "charaters",
          href: "#",
        },
        {
          title: "comics",
          href: "#",
        },
        {
          title: "movies",
          href: "#",
        },
        {
          title: "tv",
          href: "#",
        },
        {
          title: "games",
          href: "#",
        },
        {
          title: "collctibles",
          href: "#",
        },
        {
          title: "video",
          href: "#",
        },
        {
          title: "fans",
          href: "#",
        },
        {
          title: "news",
          href: "#",
        },
        {
          title: "shop",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.container {
  width: 960px;
  margin: auto;
}
nav {
  display: flex;
  justify-content: space-between;
  .logo-container {
    width: 60px;
  }
  img {
    width: 100%;
  }
}

ul {
  display: flex;
  list-style-type: none;
  align-items: center;
  margin: 0;
  li {
    padding: 10px;
  }
}
</style>