<template>
  <div class="servicesWrapper" id="services">
    <h2>services</h2>
    <ul class="services__list">
      <li>DESIGN</li>
      <li>STRATEGY</li>
      <li>PROTYPING</li>
      <li>RESEARCH</li>
    </ul>
    <div class="paragraphs">
      <p>
        Hoodie leggings offal, heirloom lo-fi pug freegan put a bird on it hella crucifix authentic
        beard biodiesel letterpress salvia. Man bun direct trade PBR&B small batch biodiesel
        meditation, roof party letterpress beard tumblr. Air plant shabby chic helvetica
        post-ironic messenger bag kickstarter.
      </p>
      <p>
        Fam crucifix offal, vaporware blue bottle hashtag brunch.
        Succulents ennui synth letterpress. Organic next level freegan, viral lumbersexual
        ennui kinfolk. Twee fixie bitters pop-up, roof party deep v 3 wolf moon irony etsy
        man braid fap jean shorts.
      </p>
      <img src="../assets/img.jpg" alt="Services image">
    </div>
  </div>
</template>

<script>

export default {
  name: 'Services',

};
</script>

<style lang="scss" scoped>
  .servicesWrapper {
    color: #fff;
    display: flex;
    flex-direction: column;
    padding: 20px;

    h2 {
      color: #5C26BA;
      font-size: 28px;
      grid-area: h2;
      text-align: center;
    }

    .services__list {
      list-style: none;
      grid-area: ul;
      padding: 0;
      display: flex;
      flex-direction: column;
      align-items: center;

      li {
        margin: 10px 0;
        font-size: 20px;
        letter-spacing: 2px;
      }
    }

    .paragraphs {
      display: flex;
      flex-direction: column;
      align-items: center;
      grid-area: paragraphs;

      p:first-of-type {
        grid-area: first-paragraph;
      }

      p:last-of-type {
        grid-area: second-paragraph;
      }

      img {
        align-self: center;
        margin-bottom: 20px;
      }
    }

    @media (min-width: 768px) {
      flex-wrap: wrap;
      flex-direction: row;

      h2 {
        text-align: left;
        margin-left: 40px;
        font-size: 42px;
        width: 100%;
      }

      .services__list {
        width: 50%;
        display: flex;
        flex-direction: column;
        align-items: center;

        li {
          font-size: 26px;
          margin: 20px 0;
        }
      }

      .paragraphs {
        width: 50%;
        flex-wrap: wrap;
        flex-direction: row;
        align-items: flex-start;

        p:first-of-type {
          width: 100%;
          order: 0;
        }

        p:last-of-type {
          width: calc(50% - 20px);
          order: 2;
          padding: 10px;
        }

        img {
          max-width: 50%;
          order: 1;
          object-fit: contain;
        }

      }
    }
  }
</style>
