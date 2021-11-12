<template>
  <footer>
    <div class="bg-footer">
      <div class="footer-container">
        <img class="logo-big" src="../assets/dc-logo-bg.png" alt="" />
        <div class="footer-list-container">
          <div class="footer-col">
            <h2>dc comics</h2>
            <ul>
              <li>Charatters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Game</li>
              <li>Video</li>
              <li>News</li>
            </ul>

            <h2>Shop</h2>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
          </div>
          <div class="footer-col">
            <h2>dc</h2>
            <ul>
              <li>Terms Of Use</li>
              <li>Privacy policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
          </div>
          <div class="footer-col">
            <h2>sites</h2>
            <ul>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="bg-footer-dark">
      <div class="footer-container footer-link">
        <button class="sign-btn">Sign-up now!</button>
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

  .bg-footer {
    background-image: url(../assets/footer-bg.jpg);
    background-size: cover;
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
        margin-bottom: 10px;
      }
      ul {
        padding-left: 0px;
        list-style-type: none;
        margin-bottom: 10px;
        li {
          color: #959595;
          font-size: 16px;
          line-height: 20px;
        }
      }
    }
  }
}
.bg-footer-dark {
  background-color: #303030;
  position: relative;

  .footer-link {
    display: flex;
    justify-content: space-between;

    .social-container {
      display: flex;
      align-items: center;

      h1 {
        color: #0282f9;
        text-transform: uppercase;
        font-size: 20px;
        padding-right: 25px;
      }

      .social-icon-container {
        img {
          padding: 0 5px;
        }
      }
    }
  }
  .sign-btn {
    border: 3px solid #0282f9;
    background-color: transparent;
    color: white;
    display: flex;
    align-items: center;
    text-align: center;
    padding: 10px 20px;
    text-transform: uppercase;
  }
}
</style>