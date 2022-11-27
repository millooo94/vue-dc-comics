<template>
  <div>
    <section class="jumbotron">
      <div class="current-series">CURRENT SERIES</div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'HeaderJumbotron',
  props: {
    jumbotron: Object,
  },
};
</script>

<style lang="scss" scoped>
.jumbotron {
  position: relative;
  height: 21.5rem;
  background-image: url('../img/jumbotron.jpg');
  background-size: cover;
}
.current-series {
      background-color: #0282f9;
      font-size: 1.2rem;
      font-weight: bold;
      color: white;
      position: absolute;
      left: 9.5rem;
      bottom: -19.2px;
      z-index: 10;
      padding: .6rem 1.4rem;
    }
</style>
