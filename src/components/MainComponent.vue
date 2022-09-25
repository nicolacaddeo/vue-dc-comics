<template>
  <main>
    <div id="cards-container">
      <CardComponent v-for="card, i in cards" :key="card" 
      :imgUrl = 'cards[i].thumb'
      :price = 'cards[i].price'
      :title = 'cards[i].series'
      :subTitle = 'cards[i].type' />
    </div>
  </main>
</template>

<script>
  import CardComponent from './CardComponent.vue';
  import {cards} from '@/data/cards_data.js';

 export default {
    name: "MainComponent",
    data() {
        return {
            cards
        };
    },
    components: { CardComponent }
}
</script>

<style scoped lang="scss">
  main {
    min-height: 55vh;
    padding: 2rem;
    background-color: #1c1c1c;
    color: #fff;
    
    #cards-container {
      width: 80%;
      margin: 0 auto;
      display: flex;
    }
  }
</style>
      
        
  