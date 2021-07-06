<template>
  <div class="welcome_page_container">
    <div class="welcome">
      <div class="welcome_bg_color"></div>
      <div class="welcome_bg_footer"></div>
      <div class="social_bg"></div>
      <div class="welcome_bg_footer-mini"></div>
      <div class="welcome_text">
        <h1>Welcome to veryfy</h1>
        <p>Fastest way to secure your business engine.</p>
        <p>Get started now.</p>
      </div>
      <div class="btns">
        <button class="btn" id="get_started">Get Started</button>
        <div class="store_container">
          <img src="../assets/stores.png" class="store" alt="go to store" />
        </div>
        <div class="social_container">
          <img src="../assets/facebook.png" class="social" alt="facebook" />
          <img src="../assets/instagram.png" class="social" alt="facebook" />
          <img src="../assets/linkedin.png" class="social" alt="facebook" />
          <img src="../assets/twitter.png" class="social" alt="facebook" />
        </div>
        <div class="laptop_container">
          <img src="../assets/lap.png" class="laptop" alt="welcome laptop" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.welcome_page_container {
  position: relative;
  color: white;
  width: 100%;
  overflow: hidden;
  padding-top: 30px;
  padding-bottom: 100px;
  z-index: -1;
  background: #fcf8f8;
}

.welcome_bg_color {
  width: 200%;
  position: absolute;
  top: -180px;
  left: -50%;
  background: #1a1357;
  border-radius: 50%;
  height: 500px;
  z-index: -1;
}

.welcome_text {
  z-index: 100;
  margin-bottom: 20px;
}

.welcome_text > p {
  margin: 0;
}

.social_bg {
  display: none;
}

.welcome_bg_footer {
  width: 50%;
  position: absolute;
  bottom: -150px;
  right: -40px;
  z-index: -1;
  border-radius: 50%;
  height: 200px;
  background: #1a1357;
}

.welcome_bg_footer-mini {
  width: 30%;
  position: absolute;
  bottom: -100px;
  right: 80px;
  z-index: -1;
  border-radius: 50%;
  height: 120px;
  background: #1a1357;
}

.store_container {
  z-index: 100;
  margin-top: 20px;
}

.store {
  width: 250px;
  height: 50px;
}

.social_container {
  margin-top: 10px;
}

.social {
  margin-right: 10px;
  border-radius: 20px;
  background: green;
  width: 30px;
}

.laptop_container {
  padding-top: 70px;
}

.laptop {
  width: 300px;
}

@media (min-width: 768px) {
  .welcome_bg_color {
    width: 500px;
    top: -120px;
    /* left: -20%; */
    left: -150px;
    height: 600px;
  }

  .welcome {
    position: relative;
    text-align: left;
    padding-top: 150px;
    width: 100%;
    margin-left: 50px;
  }

  .welcome_text > h1 {
    font-weight: 900;
    margin-left: 20px;
  }

  .social_bg {
    display: block;
    position: absolute;
    top: 360px;
    left: -100px;
    width: 300px;
    height: 150px;
    border-radius: 50%;
    background: #fcf8f8;
    z-index: -1;
  }

  .welcome_bg_footer {
    width: 40%;
    position: absolute;
    bottom: -230px;
    right: -40px;
    z-index: -1;
    border-radius: 50%;
    height: 200px;
    background: #1a1357;
  }

  .welcome_bg_footer-mini {
    width: 30%;
    position: absolute;
    bottom: -200px;
    right: 150px;
    z-index: -1;
    border-radius: 50%;
    height: 120px;
    background: #1a1357;
  }

  .store_container {
    z-index: 100;
    margin-top: 30px;
  }

  .store {
    width: 250px;
    height: 30px;
  }

  .social_container {
    margin-top: 30px;
  }

  .social {
    margin-top: 10px;
    margin-right: 10px;
    border-radius: 20px;
    background: green;
    width: 30px;
  }

  .laptop_container {
    position: absolute;
    top: 80px;
    right: 80px;
  }
}

@media (min-width: 990px) {
  .welcome_bg_color {
    width: 640px;
    top: -120px;
    left: -250px;
    height: 600px;
  }
  .welcome {
    width: 100%;
    margin-left: 100px;
  }

  .social_bg {
    display: block;
    position: absolute;
    top: 360px;
    left: -150px;
    width: 35%;
    height: 150px;
  }

  .social_container {
    margin-top: 30px;
  }

  .laptop_container {
    right: 20%;
  }

  .welcome_bg_footer {
    width: 30%;
  }
}

@media (min-width: 1240px) {
  .welcome_bg_color {
    width: 65%;
    top: -140px;
    left: -320px;
    height: 650px;
  }
  .welcome {
    width: 100%;
    margin-left: 90px;
  }

  .welcome_text,
  .welcome_text,
  .btns {
    margin-left: -30px;
  }

  .social_bg {
    display: block;
    position: absolute;
    top: 350px;
    left: -200px;
    width: 40%;
    height: 200px;
  }

  .welcome_text,
  .btns {
    padding-left: 50px;
  }

  .welcome_text > h1 {
    font-size: 3rem;
  }

  .social_container {
    margin-top: 30px;
  }

  .laptop_container {
    right: 25%;
  }

  .welcome_bg_footer {
    width: 25%;
    right: 60px;
    bottom: -180px;
  }

  .welcome_bg_footer-mini {
    width: 20%;
    bottom: -220px;
    right: 300px;
    height: 150px;
  }

  .laptop {
    width: 450px;
  }
}

@media (min-width: 1440px) {
  .welcome_bg_color {
    width: 55%;
    top: -140px;
    left: -300px;
    height: 650px;
  }

  .welcome {
    width: 100%;
    margin-left: 80px;
  }

  .social_bg {
    display: block;
    position: absolute;
    top: 350px;
    left: -180px;
    width: 30%;
    height: 220px;
  }

  .welcome_text > h1 {
    margin-left: 5px;
  }
}

@media (min-width: 1800px) {
  .welcome_bg_color {
    width: 50%;
    top: -140px;
    left: -300px;
    height: 650px;
  }

  .welcome {
    width: 100%;
    margin-left: 80px;
  }

  .social_bg {
    display: block;
    position: absolute;
    top: 350px;
    left: -180px;
    width: 30%;
    height: 220px;
  }

  .laptop {
    width: 500px;
  }

  .welcome_text,
  .welcome_text,
  .btns {
    margin-left: 100px;
  }

  .welcome_text > h1 {
    margin-left: 5px;
  }

  .laptop_container {
    right: 30%;
  }

  .welcome_bg_footer {
    width: 20%;
    right: 30px;
    bottom: -180px;
  }

  .welcome_bg_footer-mini {
    width: 20%;
    bottom: -220px;
    right: 300px;
    height: 150px;
  }
}
</style>
