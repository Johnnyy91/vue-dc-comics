<template>
  <div id="app">
    <HeaderComponent />
    <SectionMainComponent :cards='dates'/>
    <SecondSectionComponent />
    <FooterComponent />
    <SecondFooterComponent />
    
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import SectionMainComponent from './components/SectionMainComponent.vue';
import SecondSectionComponent from './components/SecondSectionComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
import SecondFooterComponent from './components/SecondFooterComponent.vue';
import {dates} from './data.js/data.js'


export default {
  name: 'App',
  data(){
    return {dates}
  },
  components: {
    HeaderComponent,
    SectionMainComponent,
    SecondSectionComponent,
    FooterComponent,
    SecondFooterComponent
}
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
} 

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
