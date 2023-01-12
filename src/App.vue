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
  text-align: center;
}
nav {
  padding: 1rem;
  background-color: #FA9494;

}

nav a {
  font-size: 1.2rem;
  padding: 1rem;
  color: #CFD2CF;
  text-decoration: none;
}

nav a.router-link-exact-active {
  color: #EB1D36;
}

</style>
