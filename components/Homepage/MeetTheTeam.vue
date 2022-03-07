<template>
  <div class="container">
    <div class="inner">
      <h1 class="head">Meet The Team</h1>
      <hr class="line">
      <p class="sub-head">Meet the team that  makes the process of this system fast and painless as possible to provide you with good result </p>
      <carousel-3d>
        <slide :index="0">
          <img src="~assets/img/possible.jpg" alt="">
        </slide>
        <slide :index="1">
          <img src="~assets/img/davidemaye.jpg" alt="">
        </slide>
        <slide :index="2">
          Slide 5 Content
        </slide>
        <slide :index="3">
          <img src="~assets/img/ernessy.jpg" alt="">
        </slide>
        <slide :index="4">
          Slide 4 Content
        </slide>
      </carousel-3d>
      <div class="testimonial-section">
        <div class="mark">
          <img src="~assets/img/Mask Group.png" alt="">
        </div>
        <div class="testimonial-inner">
          <div class="lhs">
            <svg width="52" height="52" viewBox="0 0 52 52" fill="none" xmlns="http://www.w3.org/2000/svg">
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
          <div class="middle">
            <p class="testimonial-text">Quick payment, quality service, easy withrawal and steady income all in one platform can't love it less,i definitely recommend it.</p>
            <p class="name">Akintan O. David</p>
          </div>
          <div class="rhs">
            <svg width="52" height="52" viewBox="0 0 52 52" fill="none" xmlns="http://www.w3.org/2000/svg">
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
import { Carousel3d, Slide } from 'vue-carousel-3d'
export default {
  components: {
    Carousel3d,
    Slide
  }
}
</script>

<style scoped>
.container {
  padding: 100px;
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
  justify-content: space-between;
  align-items: center;
  padding: 40px 10rem 0;
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
