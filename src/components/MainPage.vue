<template>
  <main>
    <div class="container">
      <div class="current-series">CURRENT SERIES</div>
      <CardMain
        v-for="objComics in Comics"
        :key="objComics.series"
        :comics="objComics"
        class="card-comics"
      />
      <button>LOAD MORE</button>
    </div>
  </main>
</template>

<script>
import CardMain from '@/components/CardMain.vue';
import Comics from '@/components/dc-comics.json';

export default {
  name: 'MainPage',
  components: {
    CardMain,
  },
  data() {
    return {
      Comics,
    };
  },
};
</script>

<style lang="scss" scoped>
main {
  background-color: #1c1c1c;
  position: relative;

  .container{
    margin: 0 auto;
    padding: 2.5rem 0 1rem 0;
    max-width: 1200px;
    display: flex;
    flex-wrap: wrap;

    .current-series {
      background-color: blue;
      position: absolute;
      top: -2%;
      padding: 1rem;
    }
    .card-comics {
      flex: 0 0 calc(100% / 6);
    }
    button {
      margin: auto;
    }
  }
}

</style>
