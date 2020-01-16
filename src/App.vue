<template>
  <div class="wrapper">
    <Header />
    <Info />
    <Gallery />
    <Panel />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Info from './components/Info.vue';
import Gallery from './components/Gallery.vue';
import Panel from './components/Panel.vue';

export default {
  name: 'App',
  components: {
    Header,
    Info,
    Gallery,
    Panel,

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
  }
</style>
