<template>
  <div class="hero">
    <div class="heroContent">
      <h1>Anytime, anywhere Learn on your schedule from any device</h1>
      <h2>
        We Believe everyone has the capcity to be creative Course Pro is a place
        where people develop their own potential
      </h2>
      <button>Let's get start</button>
    </div>
    <img src="../assets/Rectangle 25.svg" alt="" />
  </div>
  <div class="hero-bottom">
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="figureWrapper">
            <p class="title">Total Students</p>
            <p class="figure">5140</p>
          </div>
        </div>
        <div class="col">
          <div class="figureWrapper">
            <p class="title">Partners</p>
            <p class="figure">5140</p>
          </div>
        </div>
        <div class="col">
          <div class="figureWrapper">
            <p class="title">Affiliate Distribution</p>
            <p class="figure">5140</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>

<style>
.hero {
  position: relative;
  top: 90px;
  display: flex;
  margin-bottom: 50px;
}

.hero img {
  height: 500px;
  object-fit: cover;
}

.heroContent {
  background: #01cb63 0% 0% no-repeat padding-box;
  opacity: 1;
  width: 50%;
}

.heroContent h1 {
  color: white;
  text-align: left;
  font: normal normal bold 40px Noto Sans;
  width: 70%;
  margin: 30px auto;
}

.heroContent h2 {
  font-size: 20px;
  font-weight: 400;
  font-style: italic;
  width: 70%;
  margin: 30px auto;
}

.hero button {
  background: #000000 0% 0% no-repeat padding-box;
  border-radius: 10px;
  opacity: 1;
  text-align: left;
  font: normal normal normal 15px Noto Sans;
  letter-spacing: 0.5px;
  color: #ffffff;
  opacity: 1;
  position: relative;
  left: 110px;
}

.hero img {
  width: 50%;
  background-repeat: no-repeat;
  mix-blend-mode: multiply;
  opacity: 0.55;
}

.hero-bottom {
  background: url("../assets/small-bg.svg") 0% 0% no-repeat padding-box;
  height: 300px;
  padding-top: 50px;
  align-items: center;
  margin: auto;
}

.figureWrapper {
  height: auto;
}

.figureWrapper .title {
  text-align: left;
  font: normal normal bold 25px Noto Sans;
  letter-spacing: 0px;
  color: #86919d;
  opacity: 1;
}

.figureWrapper .figure {
  text-align: left;
  font: normal normal bold 45px Noto Sans;
  letter-spacing: 0px;
  color: #1f2532;
  opacity: 1;
}
</style>
