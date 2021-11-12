<template>
  <div class="card">
    <div class="img-container">
      <img :src="src" alt="" />
    </div>
    <div class="title"></div>
    <h6>{{ serie }}</h6>
  </div>
</template>

<script>
export default {
  name: "ProductCard",
  props: ["src", "prezzo", "serie", "tipo"],
};
</script>

<style lang="scss">
.card {
  width: calc(100% / 6);
  padding: 4px;
  margin-bottom: 5px;
  h6 {
    padding: 10px 0;
    color: white;
    text-transform: uppercase;
  }
  .img-container {
    width: 150px;
    height: 150px;
    overflow: hidden;
    img {
      width: 100%;
    }
  }
}
</style>