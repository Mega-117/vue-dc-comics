
<template>
  <header>
    <img src="../assets/dc-logo.png" alt="" />
    <nav>
      <ul>
        <li v-for="(item, i) in navBarItem" :key="i">{{ item.title }}</li>
      </ul>
    </nav>
  </header>
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

<style>
</style>