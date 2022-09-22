<template>
  <nav>
      <div>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <a href="#">Digital Comics</a>
      </div>
      <div>
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <a href="#">DC Merchandise</a>
      </div>
      <div>
          <img src="../assets/img/buy-comics-shop-locator.png" alt="">
          <a href="#">Subscription</a>
      </div>
      <div>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          <a href="#">Comic shop locator</a>
      </div>
      <div>
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
          <a href="#">DC power visa</a>
      </div>
    
    </nav>
</template>

<script>
export default {
    name: 'NavComponent'
}
</script>

<style scoped lang="scss">
nav {
    background-color:  #0282f9;
    height: 17vh;
    padding: 3rem 0;
    display: flex;
    justify-content: center;
    z-index: 3;
    
    div {
        display: flex;
        justify-content: center;
        align-items: center;
        
    }
    a {
        text-decoration: none;
        color: #fff;
        text-transform: uppercase;
        margin-left: .5rem;
        font-size: .9rem;
    }
    img {
        width: 20%;
    }
}
</style>    
        
    
