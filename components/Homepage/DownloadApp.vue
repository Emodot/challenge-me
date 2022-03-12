<template>
  <div class="container">
    <div class="inner">
      <h1 class="head">Download Our App</h1>
      <hr class="line">
      <p class="sub-head">The App is not yet Available, As soon as it is, we will let you know here, on your Email and On your notification bar</p>
      <div class="download-app">
        <img src="~assets/icons/app-store-logo 1.png" alt="">
        <img src="~assets/icons/google.png" alt="">
      </div>
      <div class="mobile-app-section">
        <img src="~assets/icons/mobile-apps.png" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.container {
  /* margin: 0%; */
  background-image: linear-gradient(#1DA1F2, #281AC8);
  height: 53rem;
}

.inner {
  /* padding: 0 100px 100px; */
  margin: 0;
  background-image: url('~/assets/icons/Path 4.4.png');
  background-size: contain;
  background-repeat: no-repeat;
}

.head {
  font-size: 35px;
  text-align: center;
  background-color: #fff;
}

.line {
  background-image: linear-gradient(#1DA1F2, #281AC8);
  border: none;
  width: 3rem;
  margin: 30px auto;
  border-radius: 50px;
  /* text-align: center; */
  height: 7px;
}

.sub-head {
  font-family: 'DM Sans', sans-serif;
  text-align: center;
  line-height: 30px;
  width: 40%;
  margin: 0 auto;
}

.download-app {
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 30px 0 13rem;
}

.download-app img {
  width: 7rem;
}

.mobile-app-section {
  /* background-image: url('~/assets/icons/Rectangle 319.png'); */
  text-align: center;
}

@media screen and (max-width: 600px) {
  .container {
    height: 40rem;
  }

  .inner {
    background-size: 150% 30%;
    background-position-x: center;
  }

  .head {
    font-size: 25px;
  }

  .sub-head {
    font-size: 15px;
    width: 90%;
  }

  .download-app {
    margin: 30px 0 70px;
  }

  .mobile-app-section img {
    width: 90%;
  }
}
</style>
