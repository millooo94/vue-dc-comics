<template>
  <header>
    <nav class="navbar">
      <div class="container">
        <a href="" class="img-link">
          <img
            src="@/img/dc-logo.png"
            alt="dc-logo">
        </a>
        <ul>
          <li v-for="item in arrNav" :key="item">
            <a href="">{{ item }}</a>
          </li>
        </ul>
      </div>
    </nav>
    <HeaderJumbotron />
  </header>
</template>

<script>
import HeaderJumbotron from '@/components/HeaderJumbotron.vue';

export default {
  name: 'HeaderPage',
  components: {
    HeaderJumbotron,
  },
  data() {
    return {
      arrNav: [
        'characters',
        'comics',
        'movie',
        'TV',
        'games',
        'collectibles',
        'videos',
        'fans',
        'news',
        'shop',
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.navbar {
  height: 5.5rem;
  background-color: white;
}
.container {
  margin: auto;
  max-width: 1200px;
  height: 100%;
  display: flex;
  justify-content: space-between;
}
.img-link {
  height: 100%;
  padding: .9rem;

  img {
    height: 100%;
  }
}
ul {
  height: 100%;
  display: flex;
  list-style: none;
  text-transform: uppercase;
  gap: 2rem;
  font-size: .8rem;
  font-weight: bold;
  color: #464646;
  li {
    height: 100%;
    position: relative;
    &:hover::before {
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 4px;
        background: #0282f9;
      }
    a {
      height: 100%;
      display: flex;
      align-items: center;
      text-decoration: none;
      &:visited, &:hover, &:active {
        color: inherit;
      }
    }
  }
}
</style>
