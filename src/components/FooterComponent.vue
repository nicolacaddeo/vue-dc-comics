<template>
  <footer>
    <section class="link-list"></section>
    <section class="social-actions"></section>
  </footer>
</template>

<script>
export default {
    name: 'FooterComponent'
}
</script>

<style scoped lang="scss">
    .link-list {
        min-height: 40vh;
        background-image: url('../assets/img/footer-bg.jpg');
    }
    .social-actions {
        height: 13vh;
        background-color: #303030;
    }
</style>