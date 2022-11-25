<template>
  <section class="jumbotron" />
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
  height: 21.5rem;
  background-image: url('../img/jumbotron.jpg');
  background-size: cover;
}
</style>
