<template>
  <div class="container">
    <div class="inner">
      <h1 class="head">Get Started with Challenge Me today</h1>
      <div class="signup">
        <p class="text">Sign up for a free account</p>
        <svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M2.8125 9H15.1875" stroke="#1DA1F2" stroke-linecap="round" stroke-linejoin="round" />
          <path d="M10.125 3.9375L15.1875 9L10.125 14.0625" stroke="#1DA1F2" stroke-linecap="round" stroke-linejoin="round" />
        </svg>
      </div>
      <div class="dashboard">
        <img src="~assets/img/Dashboard 1.png" alt="">
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
  padding: 100px 130px 0;
  background-color: #111827;
}

.head {
  font-size: 40px;
  font-weight: 700;
  width: 45%;
  color: #fff;
  line-height: 45px;
}

.signup {
  display: flex;
  align-items: center;
  margin-top: 20px;
}

.text {
  font-family: 'DM Sans', sans-serif;
  color: #1DA1F2;
  margin-right: 15px;
}

.dashboard {
  margin-top: 70px;
}

.dashboard img {
  width: 100%;
}

@media screen and (max-width: 600px) {
  .container {
    padding: 70px 50px 0;
  }

  .head {
    font-size: 25px;
    width: 100%;
    line-height: 30px;
  }

  .signup {
    margin-top: 10px;
  }

  .text {
    font-size: 14px;
    margin-right: 8px;
  }

  .dashboard {
    margin-top: 40px;
  }
}
</style>
