<template>
  <div class="galleryWrapper" id="gallery">
    <h2>gallery</h2>
    <p>
      Hoodie leggings offal, heirloom lo-fi pug freegan put a bird on it hella crucifix authentic
      beard biodiesel letterpress salvia. Man bun direct trade PBR&B small batch biodiesel
      meditation, roof party letterpress beard tumblr.
    </p>
  </div>
</template>

<script>

export default {
  name: 'Gallery',

};
</script>

<style lang="scss" scoped>
  .galleryWrapper {
    width: 100%;
    padding: 10px;
    background-color: #fafafa;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;


    h2 {
      color: #5C26BA;
      font-size: 30px;
    }

    p {
      color: gray;
      padding: 0 20px;
    }

    @media (min-width: 768px) {
      flex-direction: row;
      padding: 15px 20%;

      h2 {
        font-size: 42px;
        padding-right: 40px;
      }
    }
  }
</style>
