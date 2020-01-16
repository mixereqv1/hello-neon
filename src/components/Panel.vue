<template>
  <div class="panelWrapper">
    <p>
      we're open every day<br />
      from 8am - 7pm
    </p>
  </div>
</template>

<script>

export default {
  name: 'Panel',

};
</script>

<style lang="scss" scoped>
  .panelWrapper {
    background: url('../assets/panel.jpg') no-repeat center/cover;
    height: 400px;
    color: #fff;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding-left: 60px;

    p {
      margin-top: 120px;
      font-size: 32px;
    }

    @media (min-width: 768px) {
      padding-left: 120px;

      p {
        margin-top: 200px;
        font-size: 42px;
      }
    }
  }
</style>
