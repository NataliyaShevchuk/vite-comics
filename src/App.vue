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
              <img src="/img/buy-comics-subscription.png" alt="">
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
              <img src="/img/buy-comics-digital-comics.png" alt="">
            </div>
            <div class="text-box">
              <h4>DIGITAL COMICS</h4>
            </div>
          </div>

      </div>
    </div>

    <!-- Footer  -->
    <footer>
      <div class="container">

      </div>
    </footer>

    <!-- footer-banner -->
    <div class="footer-banner">
      <div class="container">
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



</style>
