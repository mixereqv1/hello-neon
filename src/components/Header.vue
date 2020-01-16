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
        <a href="#" class="nav__item">intro</a>
        <a href="#" class="nav__item">gallery</a>
        <a href="#" class="nav__item">services</a>
        <a href="#" class="nav__item">contact</a>
      </nav>
    </div>
  </div>
</template>

<script>

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
    display: flex;
    /* justify-content: center; */
    align-items: center;
    /* position: relative; */

    .innerWrapper {
      width: 95%;
      height: 95%;
      background: url('../assets/herobanner.jpg') no-repeat 50% 0%;
      background-size: cover;
      position: relative;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      & > * {
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
        font-size: 90px;
        margin-top: 140px;
        font-weight: 600;
        letter-spacing: 5px;
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
      flex-direction: column;
      padding: 5px;

      &__item {
        width: 40px;
        height: 40px;
        margin: 5px 0;
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
