<template>
  <div>
    <div class="header-container">
      <Header
        v-show="!showMobileMenu"
        @showMobileMenu="showMobileMenu = true"
      />
    </div>
    <div class="mobile-menu">
      <MobileMenu
        v-show="showMobileMenu"
        @closeMobileMenu="showMobileMenu = false"
      />
    </div>
    <div class="main-content">
      <Nuxt />
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      showMobileMenu: false
    }
  },
  watch: {
    $route () {
      // console.log(to);
      // console.log(from);
      // this.checkLogin()
      this.showMobileMenu = false
    }
  }
}
</script>

<style>

html {
  padding: 0px;
  margin: 0px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background: #F7F8FC;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

</style>
