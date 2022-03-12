<template>
  <div class="container" :class="{change_color: scrollPosition > 50}">
    <div class="logo">
      <img src="~assets/img/challengeMe-white 1.png" alt="">
    </div>
    <div class="menus">
      <nuxt-link to="/" class="menu">Home</nuxt-link>
      <nuxt-link to="about" class="menu">About Us</nuxt-link>
      <nuxt-link to="advertise" class="menu">Advertise</nuxt-link>
      <nuxt-link to="faq" class="menu">FAQ</nuxt-link>
      <nuxt-link to="contact" class="menu">Contact</nuxt-link>
    </div>
    <div class="login-signup">
      <button class="login">LOGIN</button>
      <div class="vl" />
      <button class="signup">REGISTER</button>
    </div>
    <div class="hamburger" @click="$emit('showMobileMenu')">
      <span class="bar" />
      <span class="bar" />
      <span class="bar" />
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      scrollPosition: null
    }
  },
  mounted () {
    window.addEventListener('scroll', this.updateScroll)
  },
  methods: {
    updateScroll () {
      this.scrollPosition = window.scrollY
    }
  }

}
</script>

<style scoped>
.container {
  z-index: 2;
  position: fixed;
  width: 100vw;
  display: flex;
  justify-content: space-between;
  align-items: center;
  /* background-color: black; */
  height: 110px;
  padding: 20px 100px;
}

.change_color {
  background-color: #151515;
}

.logo img {
  width: 6rem;
}

.menus {
  display: flex;
}

.menu {
  color: #fff;
  margin-left: 30px;
  cursor: pointer;
}

a.nuxt-link-exact-active,
a:hover {
  color:#1DA1F2;
}

.login-signup {
  display: flex;
  align-items: center;
}

.login {
  background-color: transparent;
  border: none;
  color: white;
  font-weight: 500;
  font-size: 14px;
  cursor: pointer;
}

.vl {
  border-left: 2px solid #fff;
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

.hamburger,
.mobile-logo {
  display: none;
}

.bar {
  display: block;
  width: 25px;
  height: 2px;
  margin: 5px auto;
  background-color: #ffffff;
}

@media screen and (max-width: 600px) {
  .container {
    padding: 20px;
  }

  .mobile-logo {
    display: block;
  }

  .hamburger {
    display: block;
    cursor: pointer;
  }

  .main-nav {
    padding : 20px 40px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: #F7F8FC;
  }

  .menus,
  .login-signup {
    display: none;
  }
}

</style>
