<template>
  <div class="wrapper">
    <Header />
    <Info />
    <Gallery />
    <Panel />
    <div class="servicesWithContact">
      <Services />
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Info from './components/Info.vue';
import Gallery from './components/Gallery.vue';
import Panel from './components/Panel.vue';
import Services from './components/Services.vue';

export default {
  name: 'App',
  components: {
    Header,
    Info,
    Gallery,
    Panel,
    Services,

  },
};
</script>

<style lang="scss" scoped>
  @import url('https://fonts.googleapis.com/css?family=Work+Sans:400,600,700&display=swap');
  *,
  *::before,
  *::after {
    box-sizing: border-box;
  }
  html {
    scroll-behavior: smooth;
  }
  .wrapper {
    font-family: 'Work Sans', sans-serif;

    .servicesWithContact {
      background: linear-gradient(#fff, #7d41ff);
    }
  }
</style>
