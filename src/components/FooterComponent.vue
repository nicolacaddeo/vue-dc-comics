<template>
  <footer>
    <section class="link-list-logo">
      <div class="container">
        <div class="link-list">
          <!-- DC COMICS, SHOP, DC, SITES -->
          <div class="list-container">
            <h3>DC COMICS</h3>
            <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>
            <h3>SHOP</h3>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
          </div>
          <div class="list-container">
            <h3>DC</h3>
            <ul>
              <li>Terms of Use</li>
              <li>Privacy Police (New)</li>
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
          <div class="list-container">
            <h3>SITES</h3>
            <ul>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
        </div>
        <div class="big-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </section>
    <section class="social-actions"></section>
  </footer>
</template>

<script>
export default {
    name: 'FooterComponent'
}
</script>

<style scoped lang="scss">
    .link-list-logo {
        min-height: 43vh;
        background-image: url('../assets/img/footer-bg.jpg');
    }
    .social-actions {
        height: 10vh;
        background-color: #303030;
        position: relative;
        z-index: 3;
    }

    .container {
      height: 43vh;
      width: 80%;
      margin: auto;
      display: flex;
      position: relative;
    }
    .link-list {
      width: 50%;
      height: 43vh;
      padding: 2.5rem;
      display: flex;
      .list-container {
        width: calc(100% / 3);
        h3 {
          color: #fff;
          margin-bottom: .9rem;
        }
        ul {
          margin-bottom: 1.5rem;
        }
        li {
          list-style-type: none;
          color: gray;
          font-size: .9rem;
          margin: .3rem 0;
        }
      }
    }
    .big-logo {
      width: 50%;
      height: 43vh;
      z-index: 0;
      position: absolute;
      right: 0;
      bottom: 25%;
    }
  </style>
        
        
        
              
      