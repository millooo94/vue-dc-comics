<template>
  <header>
    <nav>
      <a href="">
        <img src="@/img/dc-logo.png" alt="dc-logo">
      </a>
      <ul>
          <li><a href="">CHARACTERS</a></li>
          <li><a href="">COMICS</a></li>
          <li><a href="">MOVIE</a></li>
          <li><a href="">TV</a></li>
          <li><a href="">GAMES</a></li>
          <li><a href="">COLLECTIBLES</a></li>
          <li><a href="">VIDEOS</a></li>
          <li><a href="">FANS</a></li>
          <li><a href="">NEWS</a></li>
          <li><a href="">SHOP</a></li>
        </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'HeaderPage',
};
</script>

<style lang="scss" scoped>
header {
  height: 6rem;
  background-color: white;
}
nav {
  height: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  a {
    width: 5%;
    img {
      height: 100%;
      width: 100%;
    }
  }
  ul {
    height: 100%;
    display: flex;
    gap: 2rem;
    list-style: none;
    justify-content: space-between;
    font-size: .8rem;
    font-weight: bold;
    color: #464646; ;
    li {
      position: relative;
      display: flex;
      align-items: center;
      height: 100%;
      padding: 2rem 0 2rem 0;
      &:hover::before {
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 4px;
        background: blue;
      }
      a {
        text-decoration: none;
        &:visited, &:hover, &:active {
          color: inherit;
        }
      }
    }
  }
}

</style>
