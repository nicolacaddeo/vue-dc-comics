<template>
  <section class="social-actions-container">
    <div>
        <button>Sign-up now!</button>
    </div>
    <div class="social-icons">
        <h3>Follow Us</h3>
        <div>
          <img v-for="(icon, i) in socialIcons" :key="icon in socialIcons" :src="getSocialIcon(socialIcons, i)" alt="" />
        </div>
    </div>
  </section>
</template>

<script>
  import { socialIcons } from '@/data/social_icons_data';
export default {
    name: 'SocialComponent',
    data() {
      return {
        socialIcons
      }
    },
    methods: {
      getSocialIcon: function(array, i) {
        return `../assets/img/footer-${array[i]}.png`
      }
    }
  }
       

</script>
        

<style scoped lang="scss">
  $social-bg: #303030;
  $social-blue: #0282f9;
.social-actions-container {
  height: 10vh;
  background-color: $social-bg;
  position: relative;
  z-index: 3;
  display: flex;
  justify-content: space-around;
  align-items: center;

  button {
    background-color: $social-bg;
    color: #fff;
    font-size: 1rem;
    text-transform: uppercase;
    border: 2px solid $social-blue;
    padding: .8rem 1rem;
    cursor: pointer;
  }
  h3 {
    color: $social-blue;
    text-transform: uppercase;
  }
  .social-icons {
    display: flex;
  }
}
</style>
        