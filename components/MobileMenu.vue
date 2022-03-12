<template>
  <div class="mobile-menu">
    <div class="mobile-header">
      <div class="logo">
        <img src="~assets/img/blue-logo.png" alt="logo">
      </div>

      <div class="close" @click="closeMobileMenu">
        <span class="bar" />
        <span class="bar2" />
      </div>
    </div>
    <div class="menu-container">
      <nuxt-link to="/">
        Home
      </nuxt-link>
      <nuxt-link to="/about">
        About Us
      </nuxt-link>
      <nuxt-link to="/advertise">
        Advertise
      </nuxt-link>
      <nuxt-link to="/faq">
        FAQ
      </nuxt-link>
      <nuxt-link to="/contact">
        Contact
      </nuxt-link>
    </div>
    <div class="login-signup">
      <button class="login">LOGIN</button>
      <div class="vl" />
      <button class="signup">REGISTER</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    closeMobileMenu () {
      this.$emit('closeMobileMenu')
    }
  }
}
</script>

<style scoped>
/* MOBILE HEADER  */

.mobile-menu {
  z-index: 3;
  background-color: white;
  position: fixed;
  width: 100%;
}

.mobile-header {
  height: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  padding: 0 30px;
}

.logo img {
  width: 4rem;
}

.middle-section {
  display: flex;
  align-items: center;
  padding: 20px 50px;
}

.close {
  color: rgba(0, 0, 0, 0.22);
  cursor: pointer;
}

.bar,
.bar2 {
  display: block;
  width: 25px;
  height: 2px;
  margin: 5px auto;
  background-color: #101010;
}

.bar {
  transform: rotate(45deg);
  position: absolute;
}

.bar2 {
  transform: rotate(-45deg);
}

.menu-container {
  display: flex;
  flex-direction: column;
  font-size: 16px;
  width: 100%;
}

a {
  padding: 30px 40px;
  color: black;
  border: 1px solid rgba(0, 0, 0, 0.068);
}

.login-signup {
  margin: 30px auto;
  display: flex;
  justify-content: center;
  align-items: center;
}

.login {
  background-color: transparent;
  border: none;
  color: #1DA1F2;
  font-weight: 500;
  font-size: 14px;
  cursor: pointer;
}

.vl {
  border-left: 2px solid #1DA1F2;
  margin: 0 20px;
  height: 22px;
}

.signup {
  background-color: #1DA1F2;
  color: #fff;
  border: none;
  font-weight: 500;
  height: 45px;
  width: 120px;
  border-radius: 5px;
  font-size: 14px;
  cursor: pointer;
}
</style>
