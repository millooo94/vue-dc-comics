<template>
  <header>
    <nav>
      <a href="">
        <img src="@/img/dc-logo.png" alt="dc-logo">
      </a>
      <ul>
          <li>CHARACTERS</li>
          <li>COMICS</li>
          <li>MOVIE</li>
          <li>TV</li>
          <li>GAMES</li>
          <li>COLLECTIBLES</li>
          <li>VIDEOS</li>
          <li>FANS</li>
          <li>NEWS</li>
          <li>SHOP</li>
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
    li {
      display: flex;
      align-items: center;
      height: 100%;
      padding: 2rem 0 2rem 0;
      &:hover {
        border-bottom: 4px solid blue;
      }
    }
  }
}

</style>
