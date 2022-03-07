<template>
  <div v-scroll="handleScroll" class="container" :class="{change_color: scrollPosition > 50}">
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
  </div>
</template>

<script>
export default {
  data () {
    return {
      scrollPosition: null
    }
  },
  methods: {
    updateScroll () {
      this.scrollPosition = window.scrollY
    },
    mounted () {
      window.addEventListener('scroll', this.updateScroll)
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
  height: 130px;
  padding: 20px 100px;
}

.change_color {
  background-color:red;
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

</style>
