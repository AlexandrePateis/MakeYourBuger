<template>
  <Navbar :logo="logo_src" :alt="app_name" />
  <router-view/>
  <Footer />
</template>

<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'

export default {
 components:{
   Navbar,
   Footer
 },
 data(){
   return{
     logo_src: "/img/logo.png",
     app_name: "Make Your Burger"
   }
 }
}
</script>

<style>
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: sans-serif;
}
.main-container{
  margin: 50px;
  min-height: 555px;
}

h1{
  text-align: center;
  font-size: 4em;
  margin-bottom: 30px;
  color: rgb(0, 0, 0);
}
</style>
