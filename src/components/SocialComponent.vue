<template>
  <section class="social-actions">
    <div>
        <button>Sign-up now!</button>
    </div>
    <div>
        <h3>Follow Us</h3>
    </div>
  </section>
</template>

<script>
export default {
    name: 'SocialComponent'
}
</script>

<style scoped lang="scss">
.social-actions {
        height: 10vh;
        background-color: #303030;
        position: relative;
        z-index: 3;
        display: flex;
        justify-content: space-around;
    }
</style>