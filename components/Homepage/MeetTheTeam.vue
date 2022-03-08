<template>
  <div class="container">
    <div class="inner">
      <h1 class="head">Meet The Team</h1>
      <hr class="line">
      <p class="sub-head">Meet the team that  makes the process of this system fast and painless as possible to provide you with good result </p>
      <carousel-3d>
        <slide :index="0" class="slide-1">
          <p class="position">CEO/MD</p>
          <p class="username">Olajide A. Oladapo</p>
        </slide>
        <slide :index="1" class="slide-2">
          <p class="position">Chief Technology Officer</p>
          <p class="username">David Emaye</p>
        </slide>
        <slide :index="2" class="slide-3">
          <div />
        </slide>
        <slide :index="3" class="slide-4">
          <p class="position">Chief Marketing Officer</p>
          <p class="username">Ernest Ebuka</p>
        </slide>
        <slide :index="4" class="slide-5">
          <p class="position">Creative Director</p>
          <p class="username">Ajayi Possible</p>
        </slide>
      </carousel-3d>
      <div class="testimonial-section">
        <div class="mark">
          <img src="~assets/img/Mask Group.png" alt="">
        </div>
        <div class="testimonial-inner">
          <div class="lhs">
            <svg
              width="52"
              height="52"
              viewBox="0 0 52 52"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              @click="showPrevious"
            >
              <circle
                cx="26"
                cy="26"
                r="25.75"
                stroke="black"
                stroke-opacity="0.19"
                stroke-width="0.5"
              />
              <path d="M38 26L14 26" stroke="black" stroke-linecap="round" stroke-linejoin="round" />
              <path d="M20 20L14 26L20 32" stroke="black" stroke-linecap="round" stroke-linejoin="round" />
            </svg>
          </div>
          <VueSlickCarousel v-bind="settings" ref="carousel">
            <div class="middle">
              <p class="testimonial-text">Quick payment, quality service, easy withrawal and steady income all in one platform can't love it less,i definitely recommend it.</p>
              <p class="name">Akintan O. David</p>
            </div>
            <div class="middle">
              <p class="testimonial-text">
                Great Website,just like it was preached,making money as well as having fun at the same time is something i will never want to miss and this platform offers just that.
              </p>
              <p class="name">Oluwaseyi Ayomide</p>
            </div>
          </VueSlickCarousel>
          <div class="rhs">
            <svg
              width="52"
              height="52"
              viewBox="0 0 52 52"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              @click="showNext"
            >
              <circle
                cx="26"
                cy="26"
                r="25.75"
                transform="rotate(-180 26 26)"
                stroke="black"
                stroke-opacity="0.19"
                stroke-width="0.5"
              />
              <path d="M14 26L38 26" stroke="black" stroke-linecap="round" stroke-linejoin="round" />
              <path d="M32 32L38 26L32 20" stroke="black" stroke-linecap="round" stroke-linejoin="round" />
            </svg>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
import { Carousel3d, Slide } from 'vue-carousel-3d'
export default {
  components: {
    Carousel3d,
    Slide,
    VueSlickCarousel
  },
  data () {
    return {
      settings: {
        infinite: true,
        speed: 700,
        autoplay: false,
        arrows: false,
        // autoplaySpeed: 5000,
        // slidesToShow: 1,
        // slidesToScroll: 1,
        // fade: true,
        swipeToSlide: true,
        cssEase: 'linear'
      }
    }
  },
  methods: {
    showNext () {
      this.$refs.carousel.next()
    },
    showPrevious () {
      this.$refs.carousel.prev()
    }
  }
}
</script>

<style scoped>
.container {
  padding: 100px;
  width: 100vw;
}

.head {
  font-size: 35px;
  text-align: center;
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
  margin: 0 auto 100px;
}

/* CAROUSEL 3D SLIDE  */
.slide-5 {
  background-image: linear-gradient(rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.644)), url('~assets/img/possible.jpg');
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 20px 0 20px 30px;
}

.slide-1 {
  /* background-image: linear-gradient(rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.644)), url('~assets/img/possible.jpg'); */
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 20px 0 20px 30px;
}

.slide-2 {
  background-image: linear-gradient(rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.644)), url('~assets/img/davidemaye.jpg');
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 20px 0 20px 30px;
}

.slide-4 {
  background-image: linear-gradient(rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.644)), url('~assets/img/ernessy.jpg');
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 20px 0 20px 30px;
}

.position {
  color: #fff;
  font-weight: 600;
  font-size: 14px;
  margin-bottom: 4px;
}

.username {
  color: #fff;
  /* font-weight: 700; */
}

.carousel-3d-slide {
  border-radius: 10px;
  border: none;
  height: 5rem;
}

/* TESTIMONIAL SECTION  */
.testimonial-section {
  margin-top: 100px;
}

.mark {
  text-align: center;
}

.testimonial-inner {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 40px 10rem 0;
}

.lhs svg,
.rhs svg {
  cursor: pointer;
}

.slick-slider {
  width: 100%;
}

.testimonial-text {
  font-family: 'DM Sans', sans-serif;
  text-align: center;
  line-height: 30px;
  width: 60%;
  margin: auto;
}

.name {
  text-align: center;
  font-weight: 500;
  margin-top: 20px;
}
</style>
