<template>
  <footer>
    <div class="bg-footer">
      <div class="footer-container">
        <img class="logo-big" src="../assets/dc-logo-bg.png" alt="" />
        <div class="footer-list-container">
          <div class="footer-col">
            <h2>dc comics</h2>
            <ul>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
            </ul>

            <h2>Shop</h2>
            <ul>
              <li>testo testo</li>
              <li>testo testo</li>
            </ul>
          </div>
          <div class="footer-col">
            <h2>dc</h2>
            <ul>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
            </ul>
          </div>
          <div class="footer-col">
            <h2>sites</h2>
            <ul>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
              <li>testo testo</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="bg-footer-dark">
      <div class="footer-container footer-link">
        <button>Sign-up now!</button>
        <div class="social-container">
          <h1>Follow us</h1>

          <div class="social-icon-container">
            <img src="../assets/footer-facebook.png" alt="" />
            <img src="../assets/footer-periscope.png" alt="" />
            <img src="../assets/footer-pinterest.png" alt="" />
            <img src="../assets/footer-twitter.png" alt="" />
            <img src="../assets/footer-youtube.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
footer {
  overflow: hidden;
  position: relative;
}
.bg-footer {
  background-image: url(../assets/footer-bg.jpg);
  background-size: cover;
}
.footer-link {
  display: flex;
  justify-content: space-between;
}
.social-container {
  display: flex;

  h1 {
    color: white;
    text-transform: uppercase;
    font-size: 20px;
  }
  .social-icon-container {
    img {
      padding: 0 5px;
    }
  }
}
.footer-container {
  width: 960px;
  margin: auto;
  padding: 30px 0;
  img.logo-big {
    position: absolute;
    top: -150px;
    right: 140px;
    transform: scale(0.8);
  }
  .footer-list-container {
    position: relative;
    display: flex;
    .footer-col {
      margin-right: 20px;
      h2 {
        color: white;
        text-transform: uppercase;
      }
      ul {
        padding-left: 0px;
        list-style-type: none;
        li {
          color: #959595;
        }
      }
    }
  }
}
.bg-footer-dark {
  background-color: #303030;
  position: relative;
}
</style>