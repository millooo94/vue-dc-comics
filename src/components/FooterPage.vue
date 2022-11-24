<template>
  <footer>
    <section class="shop">
      <div class="container">
        <div class="block">
        <img src="@/img/buy-comics-digital-comics.png" alt="digital comics">
        <span>DIGITAL COMICS</span>
      </div>
      <div class="block">
        <img src="@/img/buy-comics-merchandise.png" alt="merchandise">
        <span>DC MERCHANDISE</span>
      </div>
      <div class="block">
        <img src="@/img/buy-comics-subscriptions.png" alt="subscriptionS">
        <span>SUBSCRIPTION</span>
      </div>
      <div class="block">
        <img src="@/img/buy-comics-shop-locator.png" alt="shop locator">
        <span>COMIC SHOP LOCATOR</span>
      </div>
      <div class="block">
        <img src="@/img/buy-dc-power-visa.svg" alt="power visa">
        <span>DC POWER VISA</span>
      </div>
      </div>
    </section>
    <section class="background">
      <div class="blocks">
          <div class="left-block">
          <h2>DC COMICS</h2>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <h2>SHOP</h2>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC collectibles</li>
          </ul>
        </div>
        <div class="center-block">
          <h2>DC</h2>
          <ul>
            <li>Terms of use</li>
            <li>Privacy Policy (New)</li>
            <li>Ad Choices</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshops</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>
        </div>
        <div class="right-block">
          <h2>SITES</h2>
          <ul>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>
        </div>
      </div>
      <img src="@/img/dc-logo-bg.png" alt="">
    </section>
    <section class="sub-footer"></section>
  </footer>
</template>

<script>
export default {
  name: 'FooterPage',
};
</script>

<style lang="scss" scoped>
body {
  position: relative;
  z-index: 10;
}
.shop {
  background-color: #0282f9;
  padding: 2.5rem;
  .container {
  max-width: 1000px;
  margin: auto;
  display: flex;
  gap: 2.5rem;
  justify-content: center;
  align-items: center;
  font-size: .7rem;
  .block {
    flex: 0 1 20%;
    display: flex;
    gap: 1rem;
    justify-content: flex-start;
    align-items: center;
    img {
      width: 20%;
    }
    span {
      width: 80%;

    }
  }
  }
}
.background {
  display: flex;
  gap: 10rem;
  background-image: url('@/img/footer-bg.jpg');
  background-size: cover;
  .blocks {
    display: flex;
    .left-block {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}
  }
  img {
    position: absolute;
    top: 13rem;
    left: 52rem;
   overflow: hidden;

  }

}
.sub-footer {
  height: 10rem;
  background-color: black;
}
</style>
