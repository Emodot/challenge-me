<template>
  <div class="container">
    <div class="inner">
      <h1 class="head">Why Choose Us?</h1>
      <hr class="line">
      <p class="sub-head">We are the number one go-to platform to make money while enjoying yourself, connect easily with like-minds, and make an unbelievable amount of Naira.</p>
      <div class="cards">
        <div class="lhs">
          <div class="card-1 shadow">
            <img src="~assets/icons/blender-front-color.png" alt="">
            <p class="card-head">Free Contest</p>
            <p class="card-text">Have no funds to compete and contest with others, Dont worry, Challenge me offers some free Contest for you to make huge some of money in a short period of time.</p>
          </div>
          <div class="card-1 shadow">
            <img src="~assets/icons/dollar-front-color.png" alt="">
            <p class="card-head">Unlimited Earning</p>
            <p class="card-text">The only limit to your earning is YOU and a lack of knowledge, Challenge Me has over five(5) different ways to make money explore it all, do proper research before taking a contest,know your best weapon and there is no limit to the amount of Naira you can make.</p>
          </div>
        </div>
        <div class="rhs">
          <div class="card-1 shadow">
            <img src="~assets/icons/target-front-color.png" alt="">
            <p class="card-head">Challenge System</p>
            <p class="card-text">Challenge me offers a system that can multiply your money 10 X Its original Amount.</p>
          </div>
          <div class="card-1 shadow">
            <img src="~assets/icons/puzzle-front-color.png" alt="">
            <p class="card-head">Fun and Entertainment</p>
            <p class="card-text">What is more fun than making money doing the things you love doing? Watch movies on your Favorite TV Streaming Platform, make money with the knowledge gained on Challenge Me, Watch your Favorite Football Club on your Favorite Streaming Platform, make money answering few simple questions about your Favorite Football Club on Challenge Me and a lot more.</p>
          </div>
        </div>
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
  padding: 100px;
  background-color: #fff;
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

.cards {
  display: flex;
  width: 100%;
  padding: 0 5rem;
}

.lhs, .rhs {
  flex-basis: 50%;
}

.card-1 {
  width: 90%;
  border: 1px solid rgba(0, 0, 0, 0.082);
  border-radius: 10px;
  padding: 30px;
  margin-bottom: 30px;
}

.card-1 img {
  width: 4rem;
}

.card-head {
  font-family: 'DM Sans', sans-serif;
  font-size: 20px;
  font-weight: 700;
  margin: 10px 0;
}

.card-text {
  font-family: 'DM Sans', sans-serif;
  line-height: 30px;
}

@media screen and (max-width: 600px) {
  .container {
    padding: 60px 20px;
  }

  .cards {
    flex-direction: column;
    padding: 0 10px;
  }

  .card-1 {
    width: 100%;
  }

  .sub-head {
    width: 90%;
    line-height: 25px;
  }

  .head {
    font-size: 25px;
  }
}
</style>
