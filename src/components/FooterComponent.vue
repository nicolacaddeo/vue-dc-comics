<template>
  <footer>
    <section class="link-list-logo">
      <div class="container">
        <div class="link-list"></div>
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
      border: 1px dashed white;
      height: 43vh;
      width: 80%;
      margin: auto;
      display: flex;
      position: relative;
    }
    .link-list {
      width: 50%;
      height: 43vh;
      
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
        
        
        