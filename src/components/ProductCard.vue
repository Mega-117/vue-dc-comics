<template>
  <div class="card">
    <div class="img-container">
      <img :src="src" alt="" />
    </div>
    <div class="title">
      <h6>{{ serie }}</h6>
    </div>
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
  width: calc((100% / 6) - 10px);

  margin-bottom: 5px;
  .title {
    width: 140px;
    h6 {
      padding: 15px 0 10px;
      color: white;
      text-transform: uppercase;
      line-height: 15px;
    }
  }
  .img-container {
    width: 140px;
    height: 140px;
    overflow: hidden;
    img {
      width: 100%;
    }
  }
}
</style>