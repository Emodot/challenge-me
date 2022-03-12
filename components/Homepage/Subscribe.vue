<template>
  <div class="container">
    <div class="inner">
      <h1 class="head">Subscribe our newsletter</h1>
      <hr class="line">
      <p class="sub-head">Subscribe to our newsletter for daily/weekly update of our challenges</p>
      <div class="email-input">
        <input id="" type="email" name="" placeholder="EMAIL">
        <button class="submit">SUBMIT</button>
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
  margin-top: 9rem;
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
  margin: 0 auto 40px;
}

.email-input {
  display: flex;
  justify-content: center;
}

input {
  border: 1px solid #1DA1F2;
  padding-left: 20px;
  height: 50px;
  width: 20rem;
  border-radius: 10px;
  margin-right: 10px;
  outline: none;
  background-color: transparent;
}

::placeholder {
  font-size: 14px;
}

.submit {
  background-color: #1DA1F2;
  color: #fff;
  width: 7rem;
  font-size: 14px;
  height: 50px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

@media screen and (max-width: 600px) {
  .container {
    width: 100%;
    padding: 50px 20px;
    margin-top: 70px;
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
