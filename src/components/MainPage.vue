<template>
  <main>
    <div class="container">
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
}
.container{
    margin: 0 auto;
    padding: 2.5rem 0 1rem 0;
    max-width: 1200px;
    display: flex;
    row-gap: 2.8rem;
    flex-wrap: wrap;
  }
.card-comics {
    flex: 0 0 calc(100% / 6);
  }

button {
    margin: auto;
    padding: .5rem 3.8rem;
    font-size: .8rem;
    font-weight: bold;
    color: white;
    background-color: #0282f9;
  }
</style>
