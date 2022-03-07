<template>
  <div class="container">
    <div class="inner">
      <div class="section-1">
        <img src="~assets/img/challengeMe-white 2.png" alt="" class="logo">
        <p class="about">ChallengeMe is set up to help people make some cool cash with their knowledge in different areas while also having quality fun.</p>
        <div class="socials">
          <img src="~assets/icons/Facebook.svg" alt="">
          <img src="~assets/icons/Twitter.svg" alt="">
          <img src="~assets/icons/Instagram.svg" alt="">
        </div>
      </div>
      <div class="section-2">
        <p class="head">Links</p>
        <p class="text">Home</p>
        <p class="text">About Us</p>
        <p class="text">Blog</p>
        <p class="text">Sell</p>
        <p class="text">Contact Us</p>
      </div>
      <div class="section-2">
        <p class="head">Links</p>
        <p class="text">Home</p>
        <p class="text">About Us</p>
        <p class="text">Blog</p>
        <p class="text">Sell</p>
        <p class="text">Contact Us</p>
      </div>
      <div class="section-2">
        <p class="head">Get in Touch</p>
        <p class="text">0802 345 6789</p>
        <p class="text">12, Address Street, Ondo, Nigeria</p>
      </div>
    </div>
    <div class="bottom-footer">
      <p class="copyright">Copyright © ChallengeMe. All Rights Reserved.</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.container {
  background-color: #151515;
  /* color: #fff; */
}

.logo {
  width: 5rem;
  margin-bottom: 10px;
}

.inner {
  display: flex;
  justify-content: space-between;
  padding: 100px 200px 50px;
}

.socials {
  margin-top: 20px;
  display: flex;
}

.socials img {
  margin-right: 10px;
}

.section-1 {
  flex-basis: 28%;
}

.head {
  color: #fff;
  margin-bottom: 35px;
}

.about {
  font-size: 14px;
  color: #A2A2A2;
  line-height: 25px;
}

.text {
  color: #A2A2A2;
  font-size: 12px;
  line-height: 25px;
  margin-bottom: 12px;
}

.bottom-footer {
  background-color: #000;
  height: 63px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.copyright {
  color: #fff;
  font-size: 12px;
}
</style>
