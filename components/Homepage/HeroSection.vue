<template>
  <div class="main">
    <VueSlickCarousel v-bind="settings">
      <div class="container-1">
        <div class="inner">
          <h1 class="head">Welcome To Challenge Me</h1>
          <h1 class="sub-head">CHALLENGE ME is a gaming platform that is born out of the passion to help people make-money by allowing them to exercise their knowledge in different field while learning more in the process and having fun with friends.</h1>
        </div>
      </div>
      <div class="container-2">
        <div class="inner">
          <h1 class="head">Welcome To Challenge Me</h1>
          <h1 class="sub-head">
            We do this by hosting, entertaining, educating and money-making Challenges that give you the oppurtunity to earn by challenging others with your knowledgeof any topic. We host challenges around Sport,History,Celebrities,Emtertainment such as Movies and Music and much more.
          </h1>
        </div>
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
  components: { VueSlickCarousel },
  data () {
    return {
      settings: {
        infinite: true,
        speed: 700,
        autoplay: true,
        arrows: false,
        autoplaySpeed: 5000,
        // slidesToShow: 1,
        // slidesToScroll: 1,
        fade: true,
        swipeToSlide: true,
        cssEase: 'linear'
      }
    }
  }
//   methods: {
//  showSlides() {
//    let slideIndex = 0
//   let i
//   let slides = document.getElementsByClassName("hero-text")
//   for (i = 0; i < slides.length i++) {
//     slides[i].style.display = "none"
//   }
//   slideIndex++
//   if (slideIndex > slides.length) {slideIndex = 1}
//   slides[slideIndex-1].style.display = "block"
//   setTimeout(showSlides, 3000) // Change image every 2 seconds
// }
//   }
}
</script>

<style scoped>
.main {
  width: 100vw;
}
.container-1 {
  background-image: linear-gradient(rgba(0,0,0,.5), rgba(0,0,0,.5)), url('~assets/img/image 3.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  height: 55rem;
  padding: 100px ;
}

.container-2 {
  background-image: linear-gradient(rgba(0,0,0,.5), rgba(0,0,0,.5)), url('~assets/img/image 4.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  height: 55rem;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 100px ;
}

.inner {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  height: 100%;
}

.head {
  font-size: 40px;
  font-weight: 700;
  line-height: 50px;
  color: white;
  margin-bottom: 10px;
}

.sub-head {
  font-size: 18px;
  font-weight: 400;
  line-height: 28px;
  width: 60%;
  color: white;
}

@media screen and (max-width: 600px) {
  .container-1,
  .container-2 {
    padding: 20px;
    height: 40rem;
    background-position: center;
  }

  .head {
    font-size: 25px;
  }

  .sub-head {
    font-size: 15px;
    width: 100%;
  }
}
</style>
