<script>

import TheNavbar from './components/TheNavbar.vue';

export default{
  components: { TheNavbar },

  data(){
    return{
      textInBlackBanner: "--> Content goes here <--",
    }
  }
}
</script>

<template>

    <!-- Navbara -->
    <TheNavbar></TheNavbar>

    <!-- Black Banner -->
    <div class="banner-black">
      <div class="container">
        <h2 class="my-h2"> {{textInBlackBanner}} </h2>
      </div>
    </div>
    <!-- Blue Banner -->
    <div class="banner-blue">
      <div class="container">
        <div class="row">
          <div class="col">
            <div class="img-box">
              <img src="/img/buy-comics-digital-comics.png" alt="">
            </div>
            <div class="text-box">
              <h4>DIGITAL COMICS</h4>
            </div>
          </div>

          <div class="col">
            <div class="img-box">
              <img src="/img/buy-comics-merchandise.png" alt="">
            </div>
            <div class="text-box">
              <h4>DC MERCHANDISE</h4>
            </div>
          </div>

          <div class="col">
            <div class="img-box">
              <img src="/img/buy-comics-subscriptions.png" alt="">
            </div>
            <div class="text-box">
              <h4>SUBSCRIPTION</h4>
            </div>
          </div>

          <div class="col">
            <div class="img-box">
              <img src="/img/buy-comics-shop-locator.png" alt="">
            </div>
            <div class="text-box">
              <h4>COMIC SHOP LOCATOR</h4>
            </div>
          </div>

          <div class="col">
            <div class="img-box">
              <img src="/img/buy-dc-power-visa.svg" alt="">
            </div>
            <div class="text-box">
              <h4>DC POWER VISA</h4>
            </div>
          </div>

      </div>
    </div>

    </div>
  <!-- Footer  -->
  <footer>
    <div class="container pad">
      <div class="row">
        <div class="col-6">
          <!-- lista dc comics  -->
          <div class="ul-container">
            <ul>
              <li>
                <h2>DC COMICS</h2>
              </li>
              <li>
                <a href="#">Characters</a>
              </li>
              <li>
                <a href="#">Comics</a>
              </li>
              <li>
                <a href="#">Movies</a>
              </li>
              <li>
                <a href="#">TV</a>
              </li>
              <li>
                <a href="#">Games</a>
              </li>
              <li>
                <a href="#">Videos</a>
              </li>
              <li>
                <a href="#">News</a>
              </li>
            </ul>

            <!-- lista SHOP  -->
            <ul>
              <li>
                <h2>SHOP</h2>
              </li>
              <li>
                <a href="#">Shop DC</a>
              </li>
              <li>
                <a href="#">Shop DC Collectibles</a>
              </li>
            </ul>
          </div>


          <!-- lista DC  -->
            <div class="ul-container">
              <ul>
                <li>
                  <h2>DC</h2>
                </li>
                <li>
                  <a href="#">Terms Of Use</a>
                </li>
                <li>
                  <a href="#">Privacy policy (New)</a>
                </li>
                <li>
                  <a href="#">Ad Choices</a>
                </li>
                <li>
                  <a href="#">Advertising</a>
                </li>
                <li>
                  <a href="#">Jobs</a>
                </li>
                <li>
                  <a href="#">Subscriptions</a>
                </li>
                <li>
                  <a href="#">Talent Workshop</a>
                </li>
                <li>
                  <a href="#">CPSC Certificates</a>
                </li>
                <li>
                  <a href="#">Ratings</a>
                </li>
                <li>
                  <a href="#">Shop Help</a>
                </li>
                <li>
                  <a href="#">Contact Us</a>
                </li>
              </ul>
            </div>

          <!-- lista Sites -->
          <div class="ul-container">
            <ul>
              <li>
                <h2>SITES</h2>
              </li>
              <li>
                <a href="#">DC</a>
              </li>
              <li>
                <a href="#">MAD Magazine</a>
              </li>
              <li>
                <a href="#">DC Kids</a>
              </li>
              <li>
                <a href="#">DC Universe</a>
              </li>
              <li>
                <a href="#">DC Power Visa</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-6 bg-img">
          <div class="img-bg-box">
            <img src="/img/dc-logo-bg.png" alt="">
          </div>
        </div>
      </div>
    </div>
  </footer>

  <!-- footer-banner -->
  <div class="footer-banner">
    <div class="container">
      <div class="inner-container">
        <div>
          <button>SIGN-UP NOW!</button>
        </div>
        <div class="social-container">
          <div class="h2-follow-us">
            <h3>FOLLOW US</h3>
          </div>
          <div class="img-box-footer">
            <a href="#"><img src="/img/footer-facebook.png" alt=""></a>
            <a href="#"><img src="/img/footer-twitter.png" alt=""></a>
            <a href="#"><img src="/img/footer-youtube.png" alt=""></a>
            <a href="#"><img src="/img/footer-pinterest.png" alt=""></a>
            <a href="#"><img src="/img/footer-periscope.png" alt=""></a>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<style lang="scss">
@use "./styles/general.scss" as *;

body{
  font-family: $font-text;
}

.banner-black{
  width: 100%;
  background-color: black;
  color: white;
  text-align: start;
  height: 100px;
}

.my-h2{
  padding: 2.2rem 0;
}

.banner-blue{
  width: 100%;
  background-color: $color-primary;
  color: white;
  height: 150px;

}

footer{
  background-image: url("./img/footer-bg.jpg");
  object-fit: cover;
  position: relative;
}

.footer-banner{
  background-color: $color-secondary;
  height: 100px;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  z-index: 1;
  right: 0;
}



</style>
