<template>
<div class="outerWrapper">
  <ul class="social">
    <a href="#" class="social__item pinterest"></a>
    <a href="#" class="social__item facebook"></a>
    <a href="#" class="social__item twitter"></a>
  </ul>
  <div class="innerWrapper">
    <img src="../assets/now.svg" alt="">
    <p>the time is</p>
    <nav class="nav">
      <a href="#intro" class="nav__item" v-smooth-scroll>intro</a>
      <a href="#gallery" class="nav__item" v-smooth-scroll>gallery</a>
      <a href="#services" class="nav__item" v-smooth-scroll>services</a>
      <a href="#contact" class="nav__item" v-smooth-scroll>contact</a>
    </nav>
  </div>
</div>
</template>

<script>
import Vue from 'vue';
import vueSmoothScroll from 'vue2-smooth-scroll';

Vue.use(vueSmoothScroll);

export default {
  name: 'Header',

};
</script>

<style lang="scss" scoped>
* {
  margin: 0;
}

.outerWrapper {
  width: 100%;
  height: 100vh;
  display: grid;
  grid-template:
    'social'50px 'innerWrapper'calc(100vh - 50px) / 1fr;

  @media (min-width: 768px) {
    grid-template:
      'social innerWrapper'100vh / 50px 1fr;
  }

  .innerWrapper {
    width: 100%;
    height: 100%;
    background: url('../assets/herobanner.jpg') no-repeat 50% 0%;
    background-size: cover;
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    &>* {
      z-index: 10;
    }

    img {
      position: absolute;
      width: 50%;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }

    p {
      color: #5C26BA;
      font-size: 50px;
      margin-top: 100px;
      font-weight: 600;
      letter-spacing: 5px;

      @media (min-width: 768px) {
        font-size: 90px;
        margin-top: 120px;
      }

      @media (min-width: 1024px) {
        font-size: 120px;
        margin-top: 150px;
      }
    }

    .nav {
      margin-top: 60px;

      &__item {
        margin: 0 10px;
        padding: 5px;
        text-decoration: none;
        color: #fff;
        font-size: 22px;
      }
    }
  }

  .social {
    display: flex;
    justify-content: center;
    padding: 0;

    @media (min-width: 768px) {
      flex-direction: column;
    }

    &__item {
      width: 40px;
      height: 40px;
      margin: 5px;
    }

    .pinterest {
      background: url('../assets/pinterest.svg') no-repeat;
    }

    .facebook {
      background: url('../assets/facebook.svg') no-repeat;
    }

    .twitter {
      background: url('../assets/twitter.svg') no-repeat;
    }
  }
}
</style>
