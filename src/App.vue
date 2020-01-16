<template>
  <div class="wrapper">
    <Header />
  </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
  name: 'App',
  components: {
    Header,

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
  .wrapper {
    font-family: 'Work Sans', sans-serif;
  }
</style>
