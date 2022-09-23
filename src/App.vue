<template>
  <div id="app">
    <HeaderComponent />
    <JumboTronComponent />
    <MainComponent />
    <NavComponent />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import JumboTronComponent from './components/JumboTronComponent.vue';
import MainComponent from './components/MainComponent.vue';
import NavComponent from './components/NavComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    JumboTronComponent,
    MainComponent,
    NavComponent,
    FooterComponent,
    
}
}
</script>

<style lang="scss">
  #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
}
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>



