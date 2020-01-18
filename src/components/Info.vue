<template>
  <div class="aboutWrapper" id="intro">
    <div class="about__text">
      <h2>we're hello studio</h2>
      <p>
        Lomo aesthetic lo-fi etsy sustainable cray.
        Typewriter knausgaard narwhal, vape af tofu occupy pour-over truffaut chillwave cred
        retro normcore vice brooklyn.
        Salvia occupy pork belly literally. 3 wolf moon echo park literally brooklyn gentrify,
        roof party seitan direct trade pickled cronut flexitarian.
        Try-hard knausgaard biodiesel keffiyeh, 90's yr flexitarian man braid pickled messenger
        bag PBR&B asymmetrical.
        Listicle vegan XOXO ugh direct trade, single-origin coffee master cleanse scenester.
        Lyft neutra godard normcore, swag tacos trust fund meh pitchfork dreamcatcher pork belly.
        <br /><br />
        Offal bitters vaporware yr small batch lomo. Narwhal put a bird on it next level,
        sriracha lyft fanny pack health goth hashtag bespoke church-key austin photo booth.
        Keytar activated charcoal pour-over, brooklyn kogi taxidermy vinyl fingerstache.
        Mumblecore pug craft beer, cliche typewriter leggings fixie pitchfork irony swag.
        Poke pabst PBR&B, paleo distillery neutra schlitz. Pop-up mustache 8-bit authentic
        fashion axe, neutra marfa blue bottle kickstarter health goth. Organic health goth lyft,
        gochujang lomo small batch fingerstache marfa hot chicken.
      </p>
    </div>
    <img src="../assets/about-img.jpg" alt="About image">
  </div>
</template>

<script>

export default {
  name: 'Info',

};
</script>

<style lang="scss" scoped>
  .aboutWrapper {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
    width: 90%;
    margin: 0 auto;

    @media (min-width: 1024px) {
      height: 100vh;
      width: 80%;
    }

    .about__text {
      width: 100%;
      padding: 5px;

      @media (min-width: 1024px) {
        width: 40%;
      }

      h2 {
        color: #5C26BA;
        font-size: 42px;
      }

      p {
        color: gray;
      }
    }

    img {
      margin-bottom: 10px;
    }
  }
</style>
