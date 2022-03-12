<template>
  <div>
    <div class="section-1">
      <div class="inner-1">
        <h1 class="head">How It Works?</h1>
        <hr class="line">
        <div class="content">
          <div class="card-container">
            <div class="card-1">
              <div class="lhs">
                <img src="~assets/img/create-account.png" alt="">
              </div>
              <div class="rhs">
                <p class="text">Create An Account</p>
                <p class="sub-text">The First Step is to Create an Account With Us</p>
              </div>
            </div>
            <div class="empty-card" />
          </div>
          <div class="card-container">
            <div class="empty-card" />
            <div class="card-2">
              <div class="lhs">
                <img src="~assets/img/choose-weapon.png" alt="">
              </div>
              <div class="rhs">
                <p class="text">Choose Your Weapon</p>
                <p class="sub-text">Your Weapon is the category you are most knowledgible about. e.g Sport</p>
              </div>
            </div>
          </div>
          <div class="card-container">
            <div class="card-1">
              <div class="lhs">
                <img src="~assets/img/enter-contest.png" alt="">
              </div>
              <div class="rhs">
                <p class="text">Enter Contest</p>
                <p class="sub-text">After Choosing your weapon or Category the next step is to Enter contest.</p>
              </div>
            </div>
            <div class="empty-card" />
          </div>
          <div class="card-container">
            <div class="empty-card" />
            <div class="card-2">
              <div class="lhs">
                <img src="~assets/img/win-earn.png" alt="">
              </div>
              <div class="rhs">
                <p class="text">Win and Earn</p>
                <p class="sub-text">After Entering The Contest ,take the Challenge ,Wait for the Other Challengers Result and Win.</p>
              </div>
            </div>
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
.section-1 {
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
  margin: 30px auto 100px;
  border-radius: 50px;
  /* text-align: center; */
  height: 7px;
}

.content {
  background-image: url('~/assets/img/Vector 1.png');
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
  /* padding-top: 50px; */
  padding: 0 10rem;
}

.card-container {
  display: flex;
  justify-content: space-between;
  width: 100%;
}

.card-1 {
  flex-basis: 50%;
  display: flex;
  align-items: center;
  margin-bottom: 30px;
}

.card-2 {
  flex-basis: 50%;
  display: flex;
  flex-direction: row-reverse;
  align-items: center;
  margin-bottom: 30px;
}

.rhs {
  width: 55%;
  background-color: #F7F8FC;
}

.text {
  font-family: 'DM Sans', sans-serif;
  font-weight: 700;
  font-size: 20px;
  margin-bottom: 10px;
}

.sub-text {
  /* font-weight: 500; */
  font-family: 'DM Sans', sans-serif;
  line-height: 25px;
  /* width: 250px; */
}

@media screen and (max-width: 600px) {
  .section-1 {
    padding: 50px 20px;
  }

  .head {
    font-size: 25px;
  }

  .content {
    background-image: none;
    padding: 0;
  }

  .card-1,
  .card-2 {
    flex-basis: 100%;
    margin-bottom: 70px;
  }

  .card-2 {
    flex-direction: row;
  }

  .text {
    font-size: 18px;
  }

  .sub-text {
   font-size: 15px;
  }

  .rhs {
    width: 100%;
  }
}
</style>
