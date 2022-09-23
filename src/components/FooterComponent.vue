<template>
  <footer>
    <section class="link-list-logo">
      <div class="container">
        <div class="link-list">
          <!-- DC COMICS, SHOP, DC, SITES -->
          <div class="list-container">
            <h3>DC COMICS</h3>
            <ul>
              <li v-for="item in dcComics" :key="item in dcComics">
                {{ item.title }}
              </li>
            </ul>
            <h3>SHOP</h3>
            <ul>
              <li v-for="item in shop" :key="item in shop">
                {{ item.title }}
              </li>
            </ul>
          </div>
          <div class="list-container">
            <h3>DC</h3>
            <ul>
              <li v-for="item in dc" :key="item in dc">
                {{ item.title }}
              </li>
            </ul>
          </div>
          <div class="list-container">
            <h3>SITES</h3>
            <ul>
              <li v-for="item in sites" :key="item in sites">
              {{ item.title }}
            </li>
            </ul>
          </div>
        </div>
        <div class="big-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </section>
    <SocialComponent />
  </footer>
</template>

<script>
import SocialComponent from './SocialComponent.vue';
import { dcComics, shop, dc, sites } from '@/data/footer_data';

export default {
    name: "FooterComponent",
    components: { SocialComponent },

    data() {
      return {
        dcComics,
        shop,
        dc,
        sites
      }
    }
}

</script>

<style scoped lang="scss">
    .link-list-logo {
        min-height: 43vh;
        background-image: url('../assets/img/footer-bg.jpg');
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

        
        
        
              
      
    

