<template>
  <Navbar/>
  <router-view/>
  <Footer/>
  
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Footer from '@/components/Footer.vue'

export default {
  
  components: {
    Navbar, Footer
  }
}


</script>

<style>
#app {
  font-family: Georgia, 'Times New Roman', Times, serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
 
  color:rgb(130, 8, 8);
  background-color: #F5EDDC;
}
h1{
  font-size: 2.5rem;
  text-align: center;
  text-shadow: 0.2rem 0.2rem 0.4rem #0b0bc4;
  margin: 1rem;
}


</style>
