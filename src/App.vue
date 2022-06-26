<template>
<div>
    <Navigation />
  <div class="app">
   
       
    <router-view />
  
 
  </div>
  <Footer></Footer>
</div>
  
</template>

<script>
import Navigation from './components/Navigation.vue'
import Footer from './components/Footer.vue'
export default {
  name: "App",
  components:{
    Navigation,
    Footer
  }
};
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  font-family: "Raleway", sans-serif;
  font-weight: 400;
}
.app{
  padding-top: 96px;
  @media (max-width:600px){
    padding-top: 18vw;
  }
}


</style>
