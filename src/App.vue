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
  font-family:Comic Sans, Comic Sans MS, cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
 
  color:rgb(130, 8, 8);
  background-color: #F5EDDC;
}
h1{
  font-size: 3.5rem;
  text-align: center;
 
  margin: 1rem;
}


</style>
