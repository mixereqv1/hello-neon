<template>
  <div class="contactWrapper" id="contact">
    <h2>contact</h2>
    <form action="#" method="post" class="contact__form">
      <div class="form__item">
        <input type="text" id="name" required>
        <label for="name">name</label>
      </div>
      <div class="form__item">
        <input type="text" id="topic" required>
        <label for="topic">topic</label>
      </div>
      <div class="form__item">
        <input type="email" id="email" required>
        <label for="email">email</label>
      </div>
      <input type="submit" value="SEND">
    </form>
    <div class="text">
      <p>say hello.</p>
      <p>
        Raclette cronut PBR&B, hoodie heirloom blog ethical migas lyft squid jean shorts pinterest
        succulents fixie synth. Literally skateboard 3 wolf moon organic shabby chic sartorial hell
        of mumblecore tbh humblebrag. Swag XOXO brunch humblebrag.
      </p>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Contact',

};
</script>

<style lang="scss" scoped>
  .contactWrapper {
    color: #fff;
    height: 500px;

    h2 {
      color: #5C26BA;
      font-size: 28px;
      text-align: center;
      grid-area: h2;
    }

    .contact__form {
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;

      .form__item {
        position: relative;
        margin-bottom: 1.5rem;
        width: 250px;
        min-width: 200px;

        input {
          font-family: 'Work Sans', sans-serif;
          width: 100%;
          background-color: transparent;
          border: 0;
          outline: none;
          color: #fff;
          padding: 10px;
          border-bottom: 1px solid rgba(#fff, .5);
          transition: border-bottom .3s ease;
        }

        label {
          position: absolute;
          top: 0;
          left: 0;
          padding-left: 13px;
          transition: transform .3s ease;
          opacity: .5;
        }

        input:focus {
          border-bottom: 1px solid #fff;
        }

        input:focus + label,
        input:valid + label {
          font-size: 12px;
          transform: translateY(-100%);
          opacity: 1;
        }
      }

      input[type=submit] {
        font-family: 'Work Sans', sans-serif;
        background-color: #fff;
        color: #5C26BA;
        font-weight: bold;
        letter-spacing: 2px;
        font-size: 16px;
        border: 0;
        border-radius: 28px;
        padding: 16px 90px;
        cursor: pointer;
      }
    }

    .text {
      p {
        padding: 0 20px;
      }

      p:first-of-type {
        text-align: center;
        font-size: 28px;
        font-weight: bold;
      }
    }

    @media (min-width: 768px) {
      display: grid;
      grid-template:
        'h2 h2' 100px
        'form text' 400px / 1fr 1fr;

      h2 {
        text-align: left;
        margin-left: 42px;
        font-size: 42px;
      }

      .text {
        padding-right: 200px;
        p {
          text-align: left;
        }
      }
    }
  }
</style>
